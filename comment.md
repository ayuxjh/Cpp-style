# 注释种类 (提倡加注释，但是不能滥注释)
* 重复代码 Repeat
* 解释代码 Explanation  
  - 解释不清楚就需要改进代码
* 标记代码 Marker
  - 提醒开发者
* 概述代码 Summary
* 意图说明 Description of the Code's Intent
* 传达代码无法表达的信息 Information that cannot possibly expressed by the code itself  
  - 版权声明、保密、参考文献

## 高效注释
* 高效的风格
* 伪代码编程减少注释时间，理清思路
* 编程风格就应该是一边注释、一遍code

## 注释技术 Commenting Techniques
**依据注释层次分类：程序、文件、子程序或单独行**
* 注释单行  
  - 避免注释行尾
  - 行尾注释用于数据声明
* 注释代码段
  - 不要重复代码，说明代码的意图
  - 代码本身要尽力做好说明，“不要注释难度大的代码，要重写它！！”  
  - 要说明“why”  
```c++ 
if(account_flag == 0)
bad: // if account flag equal 0
good: // if establishing a new account 
// 但是代码写得好的话就会显得注释多余,比如
if（account_type == AccountType.NewAccount）
```
* 注释数据声明 Commenting Data Declarations
  - 注释应给出变量名未传达的信息：单位、数值范围...  
  - 注释全局变量
  
* 注释控制结构 Commenting Control Structures 
* 注释子程序 Commenting Routines
  - 一两句话说清楚，说不清楚的话设计还有不足
  - 说明子程序的全局效果，如果修改了全局变量的话
  - 记录算法来源
* 注释类、文件和程序
  - 注释类（不太明白） 类的设计方法、接口？？？
  - 注释文件 文件中包含多个类，为什么要把它们放到一起