---
title       : 開放語料運動
subtitle    : Open Corpus Movement
author      : 謝舒凱 (Aber) and Pierre Magistry (A-Tsioh)
job         : 台大語言學研究所助理教授 (2010-)/台大語言學研究所博士後訪問 (2013-2014)
logo        : lopen.jpg
date        : 2014年11月8日
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
url         : {lib: "libraries"}
widgets     : [bootstrap, quiz, shiny, interactive, mathjax]  # {}
ext_widgets : {rCharts: [libraries/widgets/nvd3]}
mode        : selfcontained # {standalone, draft}

---
## 想法 (Two cents)

1. 語言學和開放政府的關係
2. 開放語料的意義與實作架構
3. 開放語料的未來芻議



--- bg:#FFFAF0

## 想法 (Two cents)

1. __`語言學和開放政府的關係`__
2. 開放語料的意義與實作
3. 開放語料的未來芻議


--- .dark .nobackground .quote
# 1 分鐘背景知識
### 1 minutes Linguistics


---
## 語言學是什麼? What is Linguistics ?

- 語言學要回答`語言的習得與發展`，`結構與功能`，`神經與心理機制`，`社會變異與演化過程`等。
- 經驗/計算語言學 (empirical/computational linguistics) [a.k.a. Natural Language Processing] 用電腦來幫助我們回答上述問題，並產生應用。

- (大數據中的) 語言數據（**語料**）蘊含了**文化歷史記憶，社會心理趨勢，政治輿情傾向，情緒偏好分佈，人格特質與決策行為，疾病前期徵兆等等**。 


--- 

## 語言分析與處理是資料科學的第二把刀 Linguistic analysis and Data Science

> - `Linguistic data are ubiqutous`, knowledge to be discovered, tendency to be predicted.

> - 自然語言處理 (Natural Language Processing) and 文本分析技術 (Textual Analytics) are the keys [Why? pressing `p`]

*** =pnotes
<q>
> Enormous amounts of textual information are becoming available electronically on a daily basis,...... Natural Language Processing (NLP) techniques have been playing an increasing role in extracting and managing entities and relations from text... substantially reducing the overhead of the development process.
</q>






---
## 語料是什麼 What are Linguistic Data ?


- 為了溝通與表情（情緒）達意（思維），我們所實現出來的語言資料。

- 在計算語言學（自然語言處理）的脈絡下，廣義的語料包括各項`語言資源`（字典 dictionay，詞庫 lexicon，語料庫 corpus，語法樹庫 treebank，知識本體 ontologies，等等。）




---
## 語言學與零時政府 Linguistics and Open Government

- 之間的距離沒有妳想的那麼遠。
- 數位時代下的多元與巨量趨勢，語料科學對於科學與社會的影響力正在發酵。
- 開發各種語言資訊應用，理解與推展社會進步的潛力

- 政府 >> 公民嗨客(civic hacking) >> 學界 >> 產業
> open the data >> hacking the data >> exploring the data >> data social product






---
## 想法 (Two cents)

1. 語言學和開放政府的關係
2. __`開放語料的意義與實作`__
3. 開放語料的未來芻議






---
## 台語輸入 TaigIME: A story from A-Tsioh
### 阮若打開 MOE ê Data

> Thanks to MOE's opening of its 《臺灣閩南語常用詞辭典》I could:
- turn a small experiment into an APP
- which was downloaded 10,000 times

### How `TaigIME-android` came into existence

> As a foreign student in linguistics. I noticed that many friends were using Taiwanese (Holo) in there online messages. It was either
- directly in ㄅㄆㄇㄈ
- or in 漢字 using Mandarin sounds in ㄅㄆㄇㄈ as IME...
As a computational linguist, the second option just drove me crazy.
How inconvenient is that !?! 
Can't you just use the transcription of Taiwanese sound to input 漢字 ?!?


---
## 台語輸入 TaigIME: A story from A-Tsioh

> I had the idea, but was missing the Data.... and MOE.cc found!!
> If the MOE had selected a too restrictive licence, the APP would never had made its way up to the Google Play Store, and now with the status of downloaded more than 10.000 times ! <https://github.com/a-tsioh/TaigIME-android/>

<img class='center'src="assets/img/taigiIME.png" alt="Drawing" style="width: 400px; height：200px"/>

- sadly no pull requests yet
- but quite a lot of feedback for a single man ! (I wish I had more time to spend on it)


---
## Linked Linguistic Data Movement 

[Open Linguistics] (http://linguistics.okfn.org/)

<img class='center'src="assets/img/llod-cloud.png" alt="Drawing" style="width: 500px; height：200px"/>



---

<iframe width="60" height="50" src='assets/img/lopen.png' frameborder="0" allowfullscreen></iframe>


--- .shout #demo

# [DEMO: 開放語料系統](http://lopen.linguistics.ntu.edu.tw/copens) 

<img class='center'src="assets/img/copens.png" alt="Drawing" style="width: 800px; height：250px"/>


---
## BIGLEX ：萌典的學伴（學界版）

| **Module.Variable**        | **Description**                       |
|---------------------|---------------------------------------|
| `concept.sense`     | word sense number from [Chinese Wordnet, CWN](http://lope.linguistics.ntu.edu.tw/cwn2/), please [help](http://lope.linguistics.ntu.edu.tw/cwikin/)       |
| `concept.gloss`     | sense definitions from CWN    |
| `concept.relations` | lexical semantic relations      |
| `emotion.polarity`  | polarity of descriptive emotional words|
| `emotion.location`  | location collocates of emotion  |
| `emotion.cause`     | cause collocates               |
| `emotion.result`    | resulting event collocates        |
| `emotion.time`        | time collocates        |
| `frequency.asbc`      | frequency of Sinica Corpus|
| `frequency.plurk`     | frequency of Plurk Corpus       |
| `frequency.childes`   | frequency of CHILDES Corpus  |
| `frequency.ptt`       | frequency of PTT                    |

**AND MANY MORE!** modules in progress: 情緒 發展歷程 語義 使用頻率 年紀 關係 性別 教學難易 部首概念 意類 知識本體 社會心理人格 . . . . . . . . . . . . . .  





---
  
## Goals and questions to answer 
  
我們的~~理想~~長遠目標

1. 人人都可以玩（語言）科學，只要她想。
2. 人人都可以邊玩邊練功邊貢獻社會，就算她沒在想。
3. 這可能嗎？
  
<a class="btn btn-large btn-danger" rel="popover" data-content="大家轉念願意放下，理解到知識從來就不應私有化。" data-original-title="" id='example'>很抱歉，不可能。除非</a>
<a id='example' data-content='Change directory doesn't actually change the directory. It changes the shell's idea of which directory we are in' data-original-title='Note'></a>

### 舉個例子：LOPEN 如何幫助開放國會？





---
## 立委問政行為: PART I 

#### 法條修正草案數前三十名立委


<div id = 'chart1' class = 'rChart nvd3'></div>
<script type='text/javascript'>
 $(document).ready(function(){
      drawchart1()
    });
    function drawchart1(){  
      var opts = {
 "dom": "chart1",
"width":    800,
"height":    400,
"x": "party",
"y": "freq",
"group": "gender",
"type": "multiBarChart",
"id": "chart1" 
},
        data = [
 {
 "name": "江惠貞",
"party": "國民黨",
"gender": "女",
"freq": 127 
},
{
 "name": "蔣乃辛",
"party": "國民黨",
"gender": "男",
"freq": 109 
},
{
 "name": "李俊俋",
"party": "民進黨",
"gender": "男",
"freq": 105 
},
{
 "name": "李昆澤",
"party": "民進黨",
"gender": "男",
"freq": 95 
},
{
 "name": "邱志偉",
"party": "民進黨",
"gender": "男",
"freq": 92 
},
{
 "name": "陳亭妃",
"party": "民進黨",
"gender": "女",
"freq": 87 
},
{
 "name": "劉建國",
"party": "民進黨",
"gender": "男",
"freq": 86 
},
{
 "name": "李桐豪",
"party": "親民黨",
"gender": "女",
"freq": 74 
},
{
 "name": "賴士葆",
"party": "國民黨",
"gender": "男",
"freq": 68 
},
{
 "name": "尤美女",
"party": "民進黨",
"gender": "女",
"freq": 67 
},
{
 "name": "李應元",
"party": "民進黨",
"gender": "女",
"freq": 67 
},
{
 "name": "王育敏",
"party": "國民黨",
"gender": "女",
"freq": 61 
},
{
 "name": "吳宜臻",
"party": "民進黨",
"gender": "女",
"freq": 60 
},
{
 "name": "陳其邁",
"party": "民進黨",
"gender": "男",
"freq": 60 
},
{
 "name": "丁守中",
"party": "國民黨",
"gender": "男",
"freq": 58 
},
{
 "name": "林佳龍",
"party": "民進黨",
"gender": "男",
"freq": 56 
},
{
 "name": "林淑芬",
"party": "民進黨",
"gender": "女",
"freq": 55 
},
{
 "name": "盧秀燕",
"party": "國民黨",
"gender": "女",
"freq": 54 
},
{
 "name": "蔡正元",
"party": "國民黨",
"gender": "男",
"freq": 54 
},
{
 "name": "羅淑蕾",
"party": "國民黨",
"gender": "女",
"freq": 52 
},
{
 "name": "黃偉哲",
"party": "民進黨",
"gender": "男",
"freq": 47 
},
{
 "name": "謝國樑",
"party": "國民黨",
"gender": "男",
"freq": 45 
},
{
 "name": "潘孟安",
"party": "民進黨",
"gender": "男",
"freq": 44 
},
{
 "name": "許添財",
"party": "民進黨",
"gender": "男",
"freq": 43 
},
{
 "name": "黃昭順",
"party": "國民黨",
"gender": "女",
"freq": 43 
},
{
 "name": "趙天麟",
"party": "民進黨",
"gender": "男",
"freq": 41 
},
{
 "name": "孫大千",
"party": "國民黨",
"gender": "男",
"freq": 41 
},
{
 "name": "管碧玲",
"party": "民進黨",
"gender": "女",
"freq": 41 
},
{
 "name": "吳育仁",
"party": "國民黨",
"gender": "男",
"freq": 41 
} 
]
  
      if(!(opts.type==="pieChart" || opts.type==="sparklinePlus" || opts.type==="bulletChart")) {
        var data = d3.nest()
          .key(function(d){
            //return opts.group === undefined ? 'main' : d[opts.group]
            //instead of main would think a better default is opts.x
            return opts.group === undefined ? opts.y : d[opts.group];
          })
          .entries(data);
      }
      
      if (opts.disabled != undefined){
        data.map(function(d, i){
          d.disabled = opts.disabled[i]
        })
      }
      
      nv.addGraph(function() {
        var chart = nv.models[opts.type]()
          .width(opts.width)
          .height(opts.height)
          
        if (opts.type != "bulletChart"){
          chart
            .x(function(d) { return d[opts.x] })
            .y(function(d) { return d[opts.y] })
        }
          
         
        chart
  .color([ "purple", "blue" ])
          
        

        
        
        
      
       d3.select("#" + opts.id)
        .append('svg')
        .datum(data)
        .transition().duration(500)
        .call(chart);

       nv.utils.windowResize(chart.update);
       return chart;
      });
    };
</script>

> "量化數據不能代表好壞只能參考，修正草案數多不一定較好，還請點選該立委觀看其修正草案的**內容**再作論定。" <http://ly.g0v.tw/>


---
## 表格數據與文本數據 Structured and un-structured data

* 問題在於 Data 有很多類型。

* 對於文本內容的深度分析可以增強信服力。




--- 
## 立委問政行為: PART II

DEMO

* 用語言表達來觀察價值選擇，關心主題與立場。
* `keyness` calculation


---
## 立委問政行為: PART III

> 國會測謊器：文本，論述，表情與政治 （無誠勿入）

> (語音，文本，多模態，言談語用，語言心理)

<iframe width="60" height="50" src='assets/img/microexpressions-lie-to-me.jpg' frameborder="0" allowfullscreen></iframe>




--- bg:#FFFAF0

## 想法 (Two cents)

1. 語言學和開放政府的關係
2. 開放語料的意義與實作
3. __`開放語料的未來芻議`__


---
## 從「還文於民」到「還語於民」

* 原視，公視，客語台影音文稿。
* 中央通訊社新聞。
* 各式公文宣導手冊。
* (以 NPR API 為例)


---
## 給出愈多，得到愈多

### 從基本詞彙到台灣南島語言族譜 (Austronesian linguistic phylogenetics)


<img class='center'src="assets/img/formosan.png" alt="Drawing" style="width: 500px; height：200px"/>


---
## Social Labs 

* (語言學) 實驗室要放在社會發展的脈絡。

* 詞典(dictionary) $\bowtie$ 詞庫 (lexicon) $\bowtie$ 詞網 (lex.network) $\bowtie$ 詞雲 (lex.cloud)

<img class='center'src="assets/img/cwm.png" alt="Drawing" style="width: 450px; height：150px"/>



---
## 結論：信願行 Conclusion


* <img class='center'src="assets/img/hacker.png" alt="Drawing" style="width: 350px; height：150px"/>

* Bridge the gap between the labs and the people !

* 眾籌眾包眾什麼都歡迎 Crowd (found|sourc)ing language resources for Taiwan.


---
# 謝謝大家！請幫忙！

- Slides: <http://loperntu.github.io/g0v2014lopen/>
- LOPEN project: <http://bit.ly/4lopen> 
- TaigiLex <https://g0v.hackpad.com/TaigiLex>




