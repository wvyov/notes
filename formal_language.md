---
title: 形式语言

updated: 2018-08-20

date: 2018-08-01

tags: 
  - 形式语言

categories: 
  - theory
  - language
---



字母表、字符串：

***字母表*** $\Sigma$ 为任意有限个字符的集合。   
***字符串*** 是字母表 $\Sigma$ 中元素构成的有限序列。    
字符串的**长度**等于序列的长度。特别的，长度为 0 的字符串，被称为**空串**，记为 $\epsilon$。



语言：

记，字母表 $\Sigma$ 上，所有长度为 $n$ 的字符串所组成的集合，为 $\Sigma^{n}$。特别的，记 $\{\epsilon\}$ 为 $\Sigma^{0}$。  
记，$\Sigma^{*} = \Sigma^{0}  \cup  \Sigma^{1} \cup  \Sigma^{2}  \cup \cdots$ 。则，$\Sigma^{*}$ 为字母表 $\Sigma$ 上所有字符串所组成的集合，也即，$\Sigma$ 的 Kleene 闭包。  
另，记，$\Sigma^{+} = \Sigma^{1} \cup  \Sigma^{2}  \cup \cdots$   
字母表上的 ***语言***（记为 $L$），是 $\Sigma^{*}$ 的任意子集。  
需要注意的是，$\Sigma^{*}$ 的空子集 $\emptyset$ 与 $\Sigma^{0}$（即，$\epsilon$） 是 两种不同的语言。



语言上的运算：

字符串间的运算，即，定义在语言 $L$ 上的运算。  
***连接*** 运算：$s_{1}s_{2} $ 且 $s_{1} \in, s_{2} \in L$ ，定义为两个字符串首尾相连。




语言间运算：

由于语言是 $\Sigma^{*}$ 的任意子集，所以语言间的运算，就是定义在 $\Sigma^{*}$ 的幂集上的运算。

1. 交、并、补运算。

2. 连接运算。  
   $L_{1}L_{2} = \{s_{1}s_{2} | s_{1} \in  L_{1}, s_{2} \in L_{2} \}$ 

3. 幂运算。  
   $L^{n}$，$n$ 个 $L$ 相连接。

4. 闭包运算。  
   $L^{*} = L_{0}  \cup L_{1} \cdots$  。

5. 补运算。  
   设，语言 $L \subseteq \Sigma^{*}$ ，则 $L$ 的补语言定义为 $\{s | s \in \Sigma^{*}, s \notin L \}$ 。




语言的表示（*自*）：

1. 形式文法  
   构造的。给定"产生式规则"集，从特定符号开始，不断地应用"产生式规则"，所有可以被构造出的字符串组成的集合，构成了一种语言。  
   或，描述了特定语言的文法结构。

2. 自动机  
   判定的。给定状态集及转移函数，通过接收输入字符串，不断地进行状态转移，所有可以使自动机最终处在终止状态的语言所组成的集合，构成了一种语言。

3. 正则语言  
   描述的。给定描述规则（正则表达式），构造特定“表达式”，所有可以被特定“表达式”描述的字符串所组成的集合，构成了一种语言。
   注：所有可以被正则表达式描述的语言，称为正则语言。

