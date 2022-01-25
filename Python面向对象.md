# Python面向对象  

```
class Employee:
   '所有员工的基类'
   empCount = 0
 
   def __init__(self, name, salary):
      self.name = name
      self.salary = salary
      Employee.empCount += 1
   
   def displayCount(self):
     print "Total Employee %d" % Employee.empCount
 
   def displayEmployee(self):
      print "Name : ", self.name,  ", Salary: ", self.salary
```

**类变量**：该变量值将在该类的所有实例间共享，empCount即为一个类变量  
**初始化方法（构造方法）**：创建该类的实例时会自动调用该方法，__init__()即为初始化方法  
**实例**：self代表类的实例。在定义类时必须有，但创建类时不必传入相应参数  

## 类的继承
继承语法`class派生类名(基类名)：`
子类不重写构造方法，则自动调用父类构造函数
**方法重写*：当父类函数无法满足子类需求时，可对该函数进行重写，子类实例将调用重写后的函数

**受保护的属性/函数**：`_protected`，只允许类本身与子类访问  
**私有属性/函数**：`__private`，只允许类本身访问  
