# Construct Transformed Array

## 📌 About
A simple and efficient Python function that constructs a transformed array 
from a given list of integers. Each element points to a new value based 
on its offset within the array.

## ⚙️ How it works
For each element `nums[i]`:
- If `nums[i] == 0` → result is `0`
- Otherwise → result is `nums[(i + nums[i]) % n]`

## 🚀 Usage
from solution import construct_transformed_array

nums = [2, 3, 1, 4]
print(construct_transformed_array(nums))  # [1, 4, 3, 2]

## 🧪 Test Cases
- Empty list       → []
- Single element   → [1]
- Multiple elements → [1, 4, 3, 2]

## 🛠️ Built With
- Python 3.x

## 👤 Author
Khalid – Morocco 🇲🇦
