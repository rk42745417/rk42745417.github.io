---
title: "Hello World"
date: 2023-07-27T21:46:28+08:00
draft: true
---
測試簡介

<!--more-->

## Introduction
Hello Hugo!

## What happened
原本想說要來寫新文章，東找找西找找發現好像把之前的 source code 弄丟了 orz。順便趁這個機會來轉 hugo，之前就一直聽說 hugo 很棒了。尤其可以順便研究新買的 domain 要怎麼指，以及 CI/CD 之類的。

## Tests
### Test header 2
$$\int_0^2 x^2\,dx = ?$$
The graph $G = (V, E)$ is a complete binary tree.  
Newline  
Another newline

New paragraph  
With yet another new line

Hi
$$\begin{align*}
5x &= 2 \newline
3y &= 4 \newline
5x + 3y &= 6
\end{align*}$$

Now we write some codes:
```cpp
#include<stdio.h>
int main() {
    int x = 5;
    print("%d\n", x * 3);
}
```
And some inline code: `$ sudo pacman -S hugo`

## Conclusion
總之看起來還不錯！除了一些問題以外：
- [ ] 中文字體很醜
- [ ] 在數學模式必須打 `\newline` 而不是 `\\`。
- [ ] 換行必須乖用兩個空格（其實也不算是問題就是了）
