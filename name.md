# 命名（Naming）
原则：通过名字就可以知道它的类型，而不用去找它的声明。  
<The power of naming conventions doesn’t come from the spe- cific convention chosen but from the fact that a convention exists, adding structure to the code and giving you fewer things to worry about.>  
**Rules are the Rules**  





## 通用命名规则
变量的命名要包含变量的含义和用途，尽量不使用缩写  
分类： 类型模版参数（type template parameters）  和 非类型模版参数（non-type template parameters） 

type template parameters should follow the rules for type names  
non-type template parameters should follow the rules for variable names.

## 文件名
全小写、下划线“_”相连

## 类型命名  Type Names
Type names start with a capital letter and have a capital letter for each new word, with no underscores
* classes, structs, type aliases, enums, and type template parameters   
``` c++   
// classes and structs
class UrlTable { ...
class UrlTableTester { ...
struct UrlTableProperties { ...

// typedefs
typedef hash_map<UrlTableProperties *, std::string> PropertiesMap;

// using aliases
using PropertiesMap = hash_map<UrlTableProperties *, std::string>;

// enums
enum UrlTableErrors { ...
```

## 变量名称 Variable Names
* Common Variable names  
   小写+“_”  snack_case (lowercase with underscore)
* Class Data Members
   不论静态还是非静态变量，尾部+“_”
* Struct Data Members
   

## Constant Names
 前面+k
 后面是 mixed-case

## Enumerator Names
  按照常量的命名方式, 也可以+前缀，表明出处
```C++
enum UrlTableErrors {
  kOk = 0,
  kErrorOutOfMemory,
  kErrorMalformedInput,
};
```

## Function Names
Ordinarily, functions should start with a capital letter and have a capital letter for each new word.  
特别地，setter和getter函数可以像变量一样命名
