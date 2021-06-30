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

[Markdown: Syntax][eng-doc].
[eng-doc]:http://daringfireball.net/projects/markdown/syntax

## 這是圖片測試
![unsplash 圖片](https://images.unsplash.com/photo-1573900941478-7cc800f708f3?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80)
