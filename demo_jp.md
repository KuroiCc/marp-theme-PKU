---
marp: true
theme: PKUSimple_AGU
paginate: true
math: mathjax
---
<!-- 
_class: title 
_paginate: false
-->
# タイトルはここまでが一行目ここから二行目です H1
<!-- # ここにタイトルを入力してください。 -->
## サブタイトルです  h2
### 作者　H3
#### 日付 H4

---
<!-- 
_class: content
_paginate: false 
-->
# 目次
## Content 
### **01** 基本スタイル H3
### **02** リスト
### **03** コード
### **04** 表
### **05** 数式
### **06** 画像
### **07** 段組み

---
<!-- _class: chapter-->
# **PART 01** 基本スタイル H1

---
<!-- _header: headerでタイトルを追加-->
# H1 タイトル1
## H2 タイトル2
### h3 タイトル3
#### h4 タイトル4
##### h5 タイトル5
###### h6 タイトル6
Normal
**Bold**

> 引用した内容

<!-- _footer: footerで参考文献などを追加 -->

---
<!-- _header: リスト-->

- 
- 順序なしリスト
  - 順序なしリスト
- 順序なしリスト

1. 順序付きリスト
2. 順序付きリスト
   1. 順序付きリスト
3. 順序付きリスト
   

---
<!-- _header: コード-->
# コードブロック
## Python
```python
import torch
print(torch.cuda.is_available())
```

## C++
```C++
#include <iostream>
using namespace std;
int main() {
    cout << "Hello world" << endl;
}
```

# インラインコード
これがインラインコード `print("Hello world")` 


<!--_footer: footertest-->
---
<!--_header: 表-->

| ヘッダー | ヘッダー | ヘッダー |
| -------- | -------- | -------- |
| セル     | セル     | セル     |
| セル     | セル     | セル     |

---
<!--_header: 数式-->
# インライン数式
インライン数式 $xyz_{123}$
# ブロック数式

$$

D(x) = \begin{cases}
\lim\limits_{x \to 0} \frac{a^x}{b+c}, & x<3 \\
\pi, & x=3 \\
\int_a^{3b}x_{ij}+e^2 \mathrm{d}x,& x>3 \\
\end{cases} 

$$

---
<!-- _header: 画像-->
>**コマンドが改行されると、画像も改行されます**

![img h:130px](images/PKUlogo_long_aogaku.svg) ![img w:200px](images/kenkyu_woman_seikou.png)
![img w:200px](images/kenkyu_woman_seikou.png)

---
<!--
_header: 段組み
_class: split
 -->
# 等分
<div class=columns>
<div>

## Column 1

Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas eveniet, corporis commodi vitae accusamus obcaecati dolor corrupti eaque id numquam officia velit sapiente incidunt dolores provident laboriosam praesentium nobis culpa.

</div>

<div>

## Column 2

Tempore ad exercitationem necessitatibus nulla, optio distinctio illo non similique? Laborum dolor odio, ipsam incidunt corrupti quia nemo quo exercitationem adipisci quidem nesciunt deserunt repellendus inventore deleniti reprehenderit at earum.

</div>
</div>

---
<!--
_header: 段組み
_class: split
 -->
# 等分じゃない
<div class=columns style="grid-template-columns: 30% 70%">
  <div>
    <img src="./images/sample_thss_img.png" width=100% >
  </div>
  <div>

  ## Column 2
  `grid-template-columns`を調整して、列の数と幅を調整します。
  **注意** 
  `<div>`タグ内での画像の挿入は`<img>`などのHTMLタグしか使えません
  `![img](image path)`のような構文は受け付けられませんが
  `#`構文は受け付けられます。
  </div>
</div>

---
![bg right contain](./images/sample_thss_img.png)
# 段組み2
直接bgを使って画像と文字を分割することももちろんできます
この場合、headerを使用できない可能性があります

---
<!--
_class: title
_paginate: false-->
# ありがとうございました