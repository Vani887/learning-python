# Project 1 技術筆記

這份筆記整理我在 Project 1（Dice Game）學到的 Python 基礎語法。

---

# 1️⃣ 基礎語法

## print()

用途：
印出內容到畫面

範例：

```python
print("Hello")
```

---

## input()

用途：
取得使用者輸入

範例：

```python
name = input("你的名字：")
```

注意：

* 回傳型別是 **字串 (str)**

---

# 2️⃣ 字串操作

## .lower()

用途：
把字串轉成小寫

範例：

```python
choice = input("y/n").lower()
```

原因：

使用者可能輸入：

```
Y
y
N
n
```

`.lower()` 可以統一格式方便判斷。

---

# 3️⃣ 條件判斷

## if / elif / else

用途：
根據條件執行不同程式。

範例：

```python
if choice == "y":
    print("roll dice")
elif choice == "n":
    print("exit")
else:
    print("invalid")
```

---

# 4️⃣ 迴圈

## while

用途：
重複執行程式。

範例：

```python
while True:
    print("hello")
```

`while True` 會形成 **無限迴圈**，
通常會搭配 `break` 結束。

---

# 5️⃣ 模組

## random

用途：
產生隨機數。

匯入模組：

```python
import random
```

---

## random.randint()

用途：
產生指定範圍的隨機整數。

範例：

```python
random.randint(1,6)
```

模擬骰子：

```
1 2 3 4 5 6
```

---

# 6️⃣ f-string

用途：
把變數放進字串裡。

語法：

```python
f"文字 {變數}"
```

範例：

```python
name = "Tom"
print(f"Hello {name}")
```

輸出：

```
Hello Tom
```

骰子程式例子：

```python
print(f'({die1}, {die2})')
```

如果：

```
die1 = 4
die2 = 2
```

輸出：

```
(4, 2)
```

---

# 7️⃣ Python 區塊（: + 縮排）

在 Python 中：

```
: 代表程式區塊開始
```

例如：

```python
if x > 5:
    print("big")
```

`print()` 這一行屬於 `if` 區塊。

---

# ⭐ 本專案學到的觀念

1️⃣ Python 用 **縮排 + :** 表示程式區塊
2️⃣ `input()` 回傳字串
3️⃣ `random.randint()` 可以模擬骰子
4️⃣ `f-string` 可以把變數放進字串
