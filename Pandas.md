# Pandas

## 常用函数
1.`pct_change()`：计算当前元素与前一元素的相差百分比  
2.`to_frame()`：将series对象转换成dataframe对象  
3.`rolling()`：窗口函数  
`df.rolling(window, min_periods=None, center=False, win_type=None, on=None, axis=0, closed=None)`
- window：表示时间窗的大小  
- min_periods：每个窗口最少包含的观测值数量，小于这个值的窗口结果为NA。值可以是int，默认None。offset情况下，默认为1  
- center: 把窗口的标签设置为居中，布尔型，默认False，居右  
- win_type: 窗口的类型。截取窗的各种函数。字符串类型，默认为None  
- on: 可选参数。对于dataframe而言，指定要计算滚动窗口的列。值为列名  
- axis: 默认为0，即对列进行计算  
- closed：定义区间的开闭，支持int类型的window。对于offset类型默认是左开右闭的即默认为right。可以根据情况指定为left、both等。  
**示例**  
使用移动窗口计算移动平均值：`df.rolling(window=5).mean()`  
使用移动窗口计算方差：`df.rolling(window=5).std()`  

4.**选取DataFrame的指定行和列**  
选取列并返回DataFrame类型的数据：`df[['col']]`  
选取列并返回Series类型的数据：`df['col']`  

5.**按两列的值对DataFrame进行排序**  
`sort_values(by = ['col1', 'col2'])`
