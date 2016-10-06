##CSS （Cascading Style Sheets）

目前， HTML 如果是網頁的骨頭，那 CSS 大概可以說是是網頁的肉和衣服。  
HTML 作為整個架構， CSS 為這個架構長出每個地方所需要的份量，並且為他穿上好看的衣服，  
最新的 CSS3 甚至還可以讓他有簡單的動作~（ 複雜的動作就交給JavaScript來吧! ）  
簡單來說， CSS 由兩個主要的部份構成：
###　
####selector { property : value ; }
####選擇器　 { 　 屬性 　:　 值　 ; }
###　
一是大括號外面左邊的 " 選擇器 "，二是右邊大括號內的 " 屬性與值 "，  
而大括號內可以有很多組屬性與值，並且每一組之間必須以分號區隔（分號也就是每組“屬性：值”的結尾）  
像這樣： 選擇器 { 屬性 : 值 ; 屬性 : 值 ; 屬性 : 值 ; }  
####選擇器 selector
基本上就是在 HTML 裡面那些標籤或是自己給他們的命名。  

>例如 < h1 > < body > < div > 這樣的東西，可以直接把標籤裡那串字變成選擇器，  
　　 像這樣：h1 { color : #FFFFFF ; } 是將 h1 設定顏色為白色  
　　 也可以在 HTML 幫他們命名（ class 或 id ），然後再將這名稱作為選擇器撰寫 CSS  
　　 像這樣：在HTML中　< div id="test" > XXX < /div >  
　　 　　　　在CSS中　　#test { background-color : #000000 ; }  
　　 　　　　是將 id 名為 test 的 div 設定成背景顏色為黑色。
  
####“屬性 property” 與 “值 value” 
點單地說，像是角色設定遊戲裡頭，可以把角色 “頭髮(選擇器)” “顏色(屬性)” 設定成 “紅色(值)”  
我想差不多是這個概念＠＠"...

只是它可以設定的東西多得跟牛毛一樣，所以要時常使用，時常去翻翻 W3 之類的教學資源，才會越來越熟悉～  
從顏色、版面、對齊、尺寸、變形、超連結、表格、插入圖片或影片 到 小小的動畫等等，  
各自都有一些選項可以選擇（ 做慣了平面設計的我OS. 這不就是跟 InDesign 裡面那些東西差不多嗎 XD? ）  
只是他是用語法寫出來．．．所以理解了規則之後，就不會覺得是無字天書了！

但是學來學去我覺得 最重要的 還是要靈活運用才可以，  
所以那一堆屬性雖然有得查，還是要努力的記得才比較方便啊～
###　
##選擇器的種類
W3 CSS 參考手冊裡頭有專門介紹全部的選擇器種類，先附上 link  
http://www.runoob.com/cssref/css-selectors.html  
除了上面說到的 #id 和 .class 之外，還有很多的樣貌，  
下面做一下簡單滴整理．．．  
#### #id { property : value ; } --- id 選擇器
這在上面有提到，可以在 HTML 中，為某個元素加上 id，  
而 CSS 中， id 前面一定要加上 “#”  。
>例如  
HTML中　< span id="test1" > XXX < /span >  
CSS中　　#test1 { display : block ; }

#### .class { property : value ; } --- class 選擇器
HTML 中，為某個元素加上 class，  
而 CSS 中， class 前面一定要加上 “.”  。
>例如  
HTML中　< span class="test2" > XXX < /span >  
CSS中　　.test2 { display : block ; }  
這是將名為 test2 的 span 設定成

但是 class 不像 id 只能有一個，可以在 HTML 中為某元件一次設定很多個。

>例如  
HTML中　< div class="test2 test3" > XXX < /div >  
CSS中　　.test2 { position : absolute ; }  
　　　　　.test3 { text-align : center ; }

#### * { property : value ; } --- 通用選擇器
“ * ” 是 選擇所有元素，表示當頁所有的元素都將套用此一設定。

#### element { property : value ; } --- 標籤選擇器
HTML 中的標籤（元素），也可以直接作為 CSS 選擇器  
>例如  
HTML中　< h1 > XXX < /h1 >  
CSS中　　h1 { font-size : 5em ; }

#### element element { property : value ; }

#### element , element { property : value ; }

#### element > element { property : value ; }

#### element + element { property : value ; }
