#ans0
C:\Users\user>python --version
Python 3.7.0
C:\Users\user>cmd
Microsoft Windows [版本 10.0.19045.2965]
(c) Microsoft Corporation. 著作權所有，並保留一切權利。

C:\Users\user>where python
C:\Users\user\AppData\Local\Programs\Python\Python37\python.exe

#ans1
pattern = "*+*+*+*+*+*+*+*+*+*+\n"  # 定義花紋的基本模式
# 利用字串乘法複製模式並顯示出來
print(pattern * 5, end='')  # 重複印出 5 次，因為總共有 5 列

#ans2
n = int(input())  # 讀取隊伍數量
team_counts = [int(input()) for _ in range(n)]  # 讀取每個隊伍的人數

# 計算合法隊伍數量
valid_teams = sum(count // 3 for count in team_counts if count % 3 == 0 and count != 0)

print(valid_teams)  # 輸出符合標準的隊伍總數

import random

def guess_number(target, max_attempts):
    attempts = 0
    while attempts < max_attempts:
        guess = int(input("請猜一個數字："))
        if guess == target:
            print("恭喜你，猜對了！")
            return
        elif guess < target:
            print("太低了，再猜一次！")
        else:
            print("太高了，再猜一次！")
        attempts += 1
    print("你已經猜了", max_attempts, "次了，遊戲結束。")

if __name__ == "__main__":
    x1 = 1  # 最小數字
    x2 = 100  # 最大數字
    target = random.randint(x1, x2)  # 隨機生成目標數字
    max_attempts = 5  # 最大猜測次數
    guess_number(target, max_attempts)
#ans3
1.Markdown 的語法有個主要的目的：用來作為一種網路內容的寫作用語言。
# 自我介紹

## 關於我
我是林鈺凌，一位學生，熱愛python。

## 學習領域
我專注於以下領域：
- **程式設計：** 我喜歡學習各種程式語言，目前專注於 Python
- **自然科學:**我從科學的真理中找到自我

## 聯絡方式
- **電子郵件：** 11232043@stu.tshs.tp.edu.tw

#ans4
import random

def guess_number(target, max_attempts):
    attempts = 0
    while attempts < max_attempts:
        guess = int(input("請猜一個數字："))
        if guess == target:
            print("恭喜你，猜對了！")
            return
        elif guess < target:
            print("太低了，再猜一次！")
        else:
            print("太高了，再猜一次！")
        attempts += 1
    print("你已經猜了", max_attempts, "次了，遊戲結束。")

if __name__ == "__main__":
    x1 = 1  # 最小數字
    x2 = 100  # 最大數字
    target = random.randint(x1, x2)  # 隨機生成目標數字
    max_attempts = 5  # 最大猜測次數
    guess_number(target, max_attempts)
