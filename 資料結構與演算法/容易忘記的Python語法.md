
# 容易忘記的Python語法

## For
- `遍歷`：for i in "banana"
- `要數字的`：for i in `range(1, 6)`
- `要index的`：for (index,i) in enumerate(sm)
- `多對一字典`:myDict.update(dict.fromkeys([1,2,3], [3]))

## for 和 if 的合併

- (x for x in xyz if x not in a)或是[x for x in xyz if x not in a]

```py
# 找出不在xyz中的值
a = [2,3,4,5,6,7,8,9,0]
xyz = [0,12,4,6,242,7,9]
gen = (x for x in xyz if x not in a)

for x in gen:
    print(x)
```

- `elif` 等同於 `else if `

# 做字典

```py
    d = {}
    for i in arr:
        if i in d: d[i] +=1
        else: d[i] =1
```

# int

- int沒有len值，只有str和arr才有，所以不能用int[3]之類的
- n//2：求除數
- n%2：求餘數

# list

- 增加陣列只能用append，不能用arr[n]=4 來直接指定擴充值。

# str

- str 可以直接用for把word遍歷出來，不用算長度，丟到array中
- str可以用字串相加，不用先用array處理再轉成str

```py
class Solution:
    def defangIPaddr(self, address: str) -> str:
        newString = ""
        for word in address:
            if word==".":newString += "[.]"
            else: newString += word
        return newString
```
