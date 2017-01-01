# data_science_tool 使用心得分享  
我所要分享我使用過的data science工具為D3，它的全名是Data-Driven Documents，亦即利用資料來驅動文件，它是一套JavaScript的函式庫，對於資料的視覺化是一項非常好用且方便的工具。  
  
優點：彈性大，自由度高，可依照個人需求客製化不同的圖表，生成的圖表也很漂亮 。
缺點：實作起來較繁瑣，不支援IE6、7、8，如果要導出圖形的話，必須額外的開發。  
  
我所使用的D3為cloudstich所包裝好的library，版本為v2.0.5，詳細可參閱 https://libraries.io/bower/cloudstitch-d3    
  
我利用D3來呈現世界各國城市土地面積以及人口數，資料來源取自The World Bank，圖表形式為泡泡圖。但是我將一般為圓形的泡泡圖改為正方形，因為我認為方塊更能表達出陸地一塊一塊的感覺，我選擇泡泡圖來呈現我的資料也是因為如此更能直覺地看出各個國家城市面積的差距比例。只要將滑鼠移到方塊上方即會顯示該國家的城市土地總面積，單位是平方公里，而點擊國家的名稱則會另外顯示該國家居住於城市的總人口數，單位是千。這裡我也使用到了D3的transform功能，讓數字能夠動態的顯示，表現了D3動態視覺化的強大功能。  

由於我是在cloudstich所提供之D3 in a box進行線上開發，因此我的資料內容也是使用google spreadsheet直接放在線上，不須放在本地端，只要線上編輯修改完成，頁面圖表就會跟著改變，非常的方便。此為我整理取得的資料之google spreadsheet網址：https://docs.google.com/spreadsheets/d/1esMPlwfcIR15NC7bwq97rT4-MTZ0apLzsRxbzjA9AMM/edit?usp=sharing  
  
對於D3有興趣想進一步了解及開發，可前往他們的官網 https://d3js.org/ 了解更多，或者直接欣賞他們各式各樣的範例 https://github.com/d3/d3/wiki/Gallery  
Hope you enjoy :)
