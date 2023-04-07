# jefvneo
## hchjf
### bccdjb
**njwcniq**xkwmocm
*jdnjvn*fvhi
* cendn
  * `code`
[jvwkjva](https://github.com/Jinnn92/Jinnn92/edit/main/README.md)
> fvenjgknmq3k
- vmkdamf
  - ncjkvmkoem

* box
  
  * 漸層
  
  * Padding
  
  * Grandient

* 背景
  
  * 顏色
  
  * 圖片

* float

# box
1. 漸層
2.  Padding
3. Grandient
---
# box是什麼?
html的每個元素都可被視作為一個盒子，然後可以針對這個盒子去做調整。

---
# box-sizing
``` box-sizing ``` 是設定物件尺寸的計算方式。
1. ``` box-sizing:content-box ``` (整體大小)
2. ``` box-sizing:border-box ``` （內容大小）
![bg right w:99%](https://i.imgur.com/vxm8vFhm.png)

---
* 所以在 block 元素中只要設定 ``` box-sizing:border-box; ```  就不用另外再計算padding、border 的寬度。
* 假設 width:300px, padding 就算加了 20px, border 加了4px，寬度依舊是300px。
![bg right w:99%](https://i1.kknews.cc/7ZSMA_iSst3TDMprjKJ9eMGgBC-PLnzhhv-n3YFRDUk/0.jpg)

---
# Padding
padding 的用途是設定物件邊框(border) 內與資料之間的留白空間，常見的翻譯是稱之為「內距」，讓你的資料不致於貼著邊框線。
1. **注意!** Padding 預設會增加物件的可見尺寸!
2. 若你對該物件設定了 padding 之後，padding 的空間則是會添加到 width 之外，所以物件的尺寸就變成了 「width + padding 」


---
 ``` css
/*四個值，個別指定*/
padding: 上  右  下   左;

/*三個值，左右採用同一個值，上下則分開指定*/
padding: 上   [右左]    下;

/*二個值，【上下】採用同一值，【左右】採用同一值*/
padding: [上下]   [右左];

/*一個值，【上下左右】都使用相同的值*/
padding: [上右下左];
 ``` 
---
# 漸層
1.漸層需要顏色跟角度
2. 可分為**線性漸層**跟**放射漸層**
3. 可以指定每個顏色的比例
4. 可以決定漸層位置跟大小

---
## 線性漸層linear-gradient
 ``` css
 background:linear-gradient(方向, 顏色1 位置, 顏色2 位置); 
 ``` 
 * 角度
     * 如果沒有設定角度，預設從上往下進行漸層。
 * 位置
      * 0% 表示起始邊界，100% 表示結束邊界 ( 邊界為填色的區外邊界 )。
      * 如果沒有指定參數，則會自動等比例分配。
      * 如果沒有指定第一個參數，預設 0%。
      * 如果沒有指定最後一個參數，預設 100%。
---
 * 顏色位置重疊
      * 如果兩種顏色位置重疊，結果將會直接呈現兩種顏色交界，若前後邊界沒有設定顏色，則會以最靠近該邊界的顏色補滿。
      ``` css
      background:linear-gradient(45deg, red 50%, black 50%); 
    ``` 
      * ![gradient](https://www.oxxostudio.tw/img/articles/202008/css-gradient-03.jpg)
---
## 放射漸層Radial Gradient 
``` css
background: radial-gradient( 形狀 範圍  at 中心位置, 顏色 色彩位置, 顏色 色彩位置,...);
 ```

---
1. 圓形
```css
 background:radial-gradient(circle at center,顏色1,顏色2);
```
2. 橢圓形
```css
background:radial-gradient(ellipse at center,顏色1,顏色2); 
```

![bg right w:99%](https://user-images.githubusercontent.com/115127388/230543074-7827cfe7-5992-47cb-b54f-3baeb380b614.png)

---
# 背景background
1. background-color: 背景顏色
2. background-image: 背景圖片
```css
background-color:FF0000
background-color:red; /* 背景為紅色 */

background-image: url(圖片網址);
```

---
# float語法
```css
float:浮動方向;
```

---

## none
``` css
float:none;
```
 ![be canter](https://user-images.githubusercontent.com/115127388/229823365-7920f770-768a-4621-a91c-c644154817b5.png)

---
## right
```css
float:right;
```

![be canter](https://user-images.githubusercontent.com/115127388/229823290-5747c9ed-481c-4248-a1c7-d9d6d8bd58ab.png)

---
## left
```css
float:left;
```

![be canter](https://user-images.githubusercontent.com/115127388/229823167-add28ca2-5699-470c-9dd2-337590676208.png)

---
