# Project 1 技術筆記

## 基礎語法

### print()
用途：印出內容到畫面

範例：
print("Hello")

---

### input()
用途：取得使用者輸入

範例：
name = input("你的名字：")

注意：回傳型別是字串 (str)

---

### .lower()

用途：把字串轉成小寫

範例：
choice = input().lower()

原因：
使用者可能輸入 Y 或 y

---

## 條件判斷

### if / elif / else

用途：根據條件執行不同程式

範例：

if choice == "y":
    print("roll dice")
elif choice == "n":
    print("exit")
else:
    print("invalid")

---

## 迴圈

### while

用途：重複執行程式

範例：

while True:
    print("hello")

---

## random 模組

### random.randint()

用途：產生隨機整數

範例：

random.randint(1,6)

模擬骰子

---

## f-string

用途：把變數放進字串

範例：

name = "Tom"
print(f"Hello {name}")

---

## 030526寫的程式

Dice Game

程式：

import random 

while True:
   choice = input('Roll the dice? (y/n): ').lower()
   if choice == 'y': 
      die1 = random.randint(1, 6)
      die2 = random.randint(1, 6)
      print(f'({die1}, {die2})')
   elif choice == 'n':
      print('Thanks for playing!')
      break 
   else:
      print('Invalid choice!')

---

## 030526學到的觀念

1. Python 用 **縮排 + :** 表示區塊
2. input() 回傳字串
3. random.randint 可以模擬骰子
4. f-string 可以把變數放進字串
