
### get poprty from object 獲得物件屬性的方法

#### Proprty 屬性

1. self property 自有屬性
  -  IsEnumerable(可枚舉): 可使用 Object.keys(obj), for ... in 獲取
  -  not Nnumerable(不可枚舉)


2. prototype from prototype has 繼承屬性
  - IsEnumerable(可枚舉):  可使用 for ... in 獲取
  - not Nnumerable(不可枚舉)

> getOwnPropertyNames: get all property from object 
  

#### The way to get poprty from object 獲得屬性的方法

- **Object.keys(obj)**：get all `self`'isenumerable property(可以把自有且可枚舉的屬性組成陣列)
- **for .. in** ：get all isenumerable property (可以把`自有`、`繼承`且可枚舉的屬性組成陣列)
- **getOwnPropertyNames**：get all property (可以把`自有`、`繼承`的`所有`屬性組成陣列)