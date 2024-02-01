# 語法介紹
## iostream
+ `iostream` 代表 "input-output stream"，它是用於標準輸入（standard input）和標準輸出（standard output）的一個header file
## vector
+ `vector` 在內存中連續存儲元素，這意味著它可以提供對元素的快速隨機訪問，同時也能夠動態地調整大小以容納更多元素。

### 創建一個向量
```cpp
vector<int> vec; // 創建一個空的int型向量

vector<double> vecDouble(5, 0.0); // 創建一個大小為5，初始值為0.0的double型向量

vector<string> vecString(3); // 創建一個含有3個空字符串的向量
```
### 在向量內添加元素
```cpp
vec.push_back(10); // 向vec添加一個元素10

vec.push_back(20); // 繼續添加一個元素20
```

### 訪問向量元素
```cpp
cout << vec[0]; // 輸出第一個元素，即10

cout << vec.at(1); // 輸出第二個元素，即20，使用at()方法訪問
```
### 向量大小和容量
```cpp
cout << vec.size(); // 輸出向量中元素的個數

cout << vec.capacity(); // 輸出向量當前的容量
```
### 檢查向量是否為空
```cpp
if(vec.empty()) cout << "向量是空的";
else cout << "向量不是空的";
```
### 移除向量中的元素
```cpp
vec.pop_back(); // 移除最後一個元素

vec.erase(vec.begin()); // 移除第一個元素

vec.clear(); // 清除所有元素

```
### 遍歷向量
```cpp
for(int i = 0; i < vec.size(); ++i) {
    cout << vec[i] << " ";
}
// 或者使用範圍for循環
for(auto& value : vec) {
    cout << value << " ";
}
```
### 使用迭代器遍歷
```cpp
for(auto it = vec.begin(); it != vec.end(); ++it) {
    cout << *it << " ";
}

```
## algorithm
+ `algorithm`  是一個包含許多標準算法的標頭檔案，其中一個常用的功能是 `sort` 函數，用於對數據進行排序。
### 使用 sort 函數對 vector 進行排序
```cpp
vector<int> vec = {4, 1, 3, 2, 5};
sort(vec.begin(), vec.end()); // 將向量從小到大排序
```
### 對部分容器進行排序
```cpp
sort(vec.begin(), vec.begin() + 3); // 只對前三個元素進行排序
```

## double
+ `double` 是一種資料型態，用於存儲雙精度浮點數，常用於科學計算、工程設計、金融分析等需要高精度浮點運算的領域

## 基本邏輯判斷
+ 或`||`、且`&&`、等於`==`

