# makedown_test0
## makedown_test1
### makedown_test2
#### makedown_test3
##### makedown_test4

## 這是文字段落測試
這是一段文字段落 1-1
這是一段文字段落 1-2

這是二段文字段落 2-1
這是二段文字段落 2-2

## 這是引用測試
> 這裡是一段引用文字

## 這是清單測試
- 這是清單
+ 這也是清單
* 這同樣是清單
    - 清單子項目 (tab來表達階層)

1. 數字型清單
2. 第二個數字清單
3. 第三個數字清單
4. 第四個數字清單
    1. 第四個數字清單的子清單 (tab來表達階層)
    2. 第四個數字清單的子清單
5. 第五個數字清單
  
## 這是函數測試
```
for (let i = 0; i < 10; i++) {
  setTimeout(function () {
    console.log('這執行第' + i + '次');
  }, 0);
}
```

```
<body>
  <p>這是一段 HTML 結構</p>
</body>
```

## 這是分隔線測試
---
***
___


## 這是表格測試
(畫表格)
| thead 1 | thrad 2 | thread 3 |
|---------|---------|----------|
| td      | td      | td       |

環境許可直接使用 HTML 的表格標籤替代 Markdown 的表格，比較方便

## 這是行內元素測試
斜體
*
_
*斜體*
_斜體_

強調
**
__
**強調**
__強調__

## 這是行內程式碼測試
`<strong>` strong `</strong>`

`var a = 0`

## 這是連結測試
<h2 id="link">連結</h2>
連結的結構略有不同，會分為前後兩個片段符號：

前者為 [ ]：中括號內需要補上連結的顯示文字。
後者為 ( )：小括號內補上的是連結路徑。

[Google](https://www.google.com.tw/)

[連結](#link)

[Markdown: Syntax][markdown-doc].

[markdown-doc]:https://github.com/othree/markdown-syntax-zhtw/blob/master/syntax.md

## 這是特殊字元自動轉換測試
在 HTML 文件中，有兩個字元需要特殊處理： `<` 和 `&` 。 `<` 符號用於起始標籤，`&` 符號則用於標記 HTML 實體，如果你只是想要使用這些符號，你必須要使用實體的形式，像是 `&lt;` 和 `&amp;`。

`&` 符號其實很容易讓寫作網路文件的人感到困擾，如果你要打「AT&T」 ，你必須要寫成「`AT&amp;T`」 ，還得轉換網址內的 `&` 符號，如果你要連結到：

    http://images.google.com/images?num=30&q=larry+bird

你必須要把網址轉成：

    http://images.google.com/images?num=30&amp;q=larry+bird

才能放到連結標籤的 `href` 屬性裡。不用說也知道這很容易忘記，這也可能是 HTML 標準檢查所檢查到的錯誤中，數量最多的。

Markdown 允許你直接使用這些符號，但是你要小心跳脫字元的使用，如果你是在HTML 實體中使用 `&` 符號的話，它不會被轉換，而在其它情形下，它則會被轉換成 `&amp;`。所以你如果要在文件中插入一個著作權的符號，你可以這樣寫：

    &copy;

Markdown 將不會對這段文字做修改，但是如果你這樣寫：

    AT&T

Markdown 就會將它轉為：

    AT&amp;T

類似的狀況也會發生在 `<` 符號上，因為 Markdown 支援 [行內 HTML](#html) ，如果你是使用 `<` 符號作為 HTML 標籤使用，那 Markdown 也不會對它做任何轉換，但是如果你是寫：

    4 < 5

Markdown 將會把它轉換為：

    4 &lt; 5

不過需要注意的是，code 範圍內，不論是行內還是區塊， `<` 和 `&` 兩個符號都*一定*會被轉換成 HTML 實體，這項特性讓你可以很容易地用 Markdown 寫 HTML code （和 HTML 相對而言， HTML 語法中，你要把所有的 `<` 和 `&` 都轉換為 HTML 實體，才能在 HTML 文件裡面寫出 HTML code。）

## 這是圖片測試
![unsplash 圖片](https://images.unsplash.com/photo-1573900941478-7cc800f708f3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80)


## reference
https://github.com/othree/markdown-syntax-zhtw/blob/master/syntax.md
https://wcc723.github.io/development/2019/11/23/ten-mins-learn-markdown/
