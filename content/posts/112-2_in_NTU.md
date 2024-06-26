---
title: "112-2 in NTU"
date: 2024-06-26T17:05:05+08:00
draft: false
---
# 引言
已經超過一年半沒碰這東西了，超好笑。111-2 跟 112-1 的學期心得都在不知不覺中忘記了，原本沒有打算要寫這篇的，但是想說最近可以分享一些最近學到的酷東西，所以就用好久不見的學期心得來重回這個地方吧！

<!--more-->

# 修課
越來越覺得修課跟休克其實是等價的了，這學期原本打算大養生的，但是被推坑了 CNS 和 FAI 後整個學期就馬不停蹄。

## 系上必修
### 機率
成績：A+
系上的大二下必修，有分單號班跟雙號班，兩個班不同老師教的東西也不一樣。單號班教的東西感覺蠻有水準的而且也很難，雙班的洪一平老師教的就是高中數學上再多一些些東西而已，實際感覺是雙班整學期教的東西單班在期中考後一點點就教完了。而因為我對數學實在沒什麼興趣，所以我就待在雙班了。單班跟雙班好像都可以轉，有一些人想好好學就會轉單班，有一些人想混就會轉雙班。

雙班有三次考試，小考、期中考與期末考，小考會在期中周之前考，期中考會在期中周後一段時間才考，期末考就在期末周考，占比分別 10%、20%、40%。小考的範圍基本上就是高中的排組，期中考就有比較多東西了，但大部分都是背誦的，而可以帶雙面大抄的情況下就是把各個 distribution 的各種結論抄起來，不過大抄要手抄的，所以可能需要準備一個多小時來抄。我們這學期課放假比較多，所以其實期末考只比期中考的範圍多了兩堂課不到六小時的課程，期末考也因此範圍基本上就是期中考的範圍，所以也沒有讀，就只是把課補完然後大抄好好做就可以了，難度不會很高，計算題居多。
作業有幾次，每次基本上就是課本題，所以就很簡單，然後也給很長的時間寫，所以基本上沒有 loading。
最後就是最精華的部分，洪老師不知道為什麼對 NFT 和數位創作特別有興趣，所以他有一個加分作業是去參加若水獎（一個把創作品鑄造成 NFT 參賽的藝術比賽）就可以加分。原本去年是根據一些規則加學期成績 1~5 分，今年變成有參賽就 1 分，做得不要太差而且作品有用到機率就加學期成績一個等第，我覺得我期末考考得很糟但因為有做加分作業所以好像也有 A+。加分作業基本上也是半天能弄完。
### 人工智慧導論
成績：A-~A+
被同學拉去修的大三必修，基本上是為了順應 AI 潮而硬加的一門必修課，看得出來教授也不怎麼想教這門課。兩個教授合教，但很果斷的切成上下半學期，教完全不一樣的東西。

前半學期是陳尚澤老師在教 Berkeley 的 introductory artificial intelligence，作業也一樣，然後老師在講課的時候切到下一頁投影片時還會停頓個幾秒鐘來看這頁在講什麼，我覺得老師這一年來第一次看到這份投影片就是上課的時候。有期中考，因為 Berkeley 那邊十年來每年的三個學期都有開這門課，所以題目來源很多，雖然沒明講但基本上就是從 Berkeley 的考古題中挑幾題來考，因為數量很多刷完沒什麼價值，基本上就是順帶的練一練考古題，難度其實不低，雖然我自己覺得實際期中考時難度沒有很高但我最後還是考炸了。

下半學期就是 vivian 老師講機器學期，就是把林軒田老師的 HTML 濃縮後講完，然後作業感覺是自己出的但出得怪怪的，期末 Project 是要實作一個能夠在德州撲克打贏助教寫的 AI 的 AI。聽說用 train 模型的方式都很糟，最後很強的那些都是用蒙地卡羅把勝率算出來後透過對德州撲克的理解來進行 heuristic。所以整學期教的東西其實都用不到期末 project，只需要你會打德州撲克，非常好的一門課。
### 專題研究
成績：A+
整學期最喜歡的，我大概去年暑假的時候問說能不能參與黎士偉老師的實驗室 meeting，而寒假的時候就問老師能不能開始做事。老師一開始丟給了我好幾個題目，我最後是選擇做嘗試把 Arm trusted execution environment 的開放原始碼實作 OPTEE 系統開機在 Arm cofidential compute architecture 中的 realm management extension 的 realm VM。 我不知道有幾個人在看完這句話後能夠理解這在幹嘛，我自己當初也是光理解題目就花了一兩個禮拜，因為有大量的背景知識，要從 Arm 的整個 confidential compute architecuture 的大觀念和一些細節相關去理解。建置環境時也花了不少努力，因為編譯執行都要在 VM 裡面做，所以編譯那些大東西往往就需要個一兩天，很感謝實驗室的機器能夠給我們用。期中大概是成功把整個環境弄好，到期末前就是開始研究怎麼開機。其實有個碩士學長也在做類似的事情，主要就是我們要把 OPTEE 會想要 call 的 secure monitor call 轉成對應的 RMI 指令（因為 realm VM 不能直接得到 EL3 的東西，畢竟他們不是在 Secure World）。實際上基本上就是啃一堆 C 和 assembly 的 code，還沒能做出什麼東西就結束了。老師也說系統類的東西往往都有很大量的背景知識，要讀懂 code 更需要耐心地 trace code，所以也鼓勵我們之後繼續做這方面的東西，我也覺得這東西雖然很難，但真的很酷，很喜歡實際操手大東西的感覺，這跟課程 project 完全不一樣。

## 系上選修
### 密碼學與資訊安全
成績：A+
蕭旭君老師開的選修課，因為上學期修過了計安想說這學期也來修更多資安方面的，可以體會到老師用心準備上課內容，而且上課內容也很有趣。作業很難但是就正常的硬課，給分也相當甜，期末 Project 是要自己做一個資安方面的貢獻，我們這組當初想題目就花了很久，最後也是感覺沒有很認真地做，可是因為另外兩個人的大腿很粗而且給分真的很甜所以好像也沒差。總之蠻推這門課的！

## 共同必修、通識、系外選修
### 水資源概論
成績：通過（原B-）
因為探索學分的六學分都沒用過，所以就隨便選了通識課。這門課教了水資源相關的各種議題，要點名，有期中考跟期末報告（雖然期中考在期末周的前一周考）。除此之外還有幾次的報告要交，報告都很自訂主題，我基本上都是把這幾堂課的東西統整一下給心得，但似乎給分蠻鬆的。期中考只要好好讀基本上都很簡單，但我沒有好好讀。期末報告我甚至睡過去了，分數被打 80%，但每一組除了上台以外還要拍影片和準備書面報告（因為一組有很多很多人），有點對不起我們這組，因為我探索仔所以我沒有花什麼心力。

### 東亞現代史
成績：通過（原 A-）
也是隨便選的通識課，但意外的老師上課很有趣，跟國高中那種歷史課很不一樣，都是從小人物的角度，去了解他們為什麼會做這些事情，從而理解當時整個大環境下的長相，很有在研究歷史的感覺。不過 loading 不小，每周都有討論課，討論課前至少要看一部指定的電影，最好還要讀指定文本，文本都是那種實體的書，然後加起來可能都有個一兩百頁或更多。我因為探索仔所以我沒讀過文本，電影甚至有好幾部也沒看，但是討論課時我就盡力地在帶大家討論（畢竟我自己沒東西可以輸出，哈），感覺給助教印象還不錯。還有四次作業要寫至少兩次，都是給一個圍繞著那幾次上課主題的題目，要寫一篇論述文，有點像是看了很多的文本和資料後，有自己的論點那種，而且文本都要有對應的參考資料。但是我沒有在讀文本，兩次都是維基跟 chatGPT 搞定，第二次的我沒看到成績，第一次的作業成績有個 A-，感覺給分很鬆，但高分可能不是我這文科笨蛋能做到的。期末報告是一個更長的論述文，要有更多自己的論點和看更多的文本，而我還是靠 chatGPT，最後卻還是有 A 字頭，所以這大概是 loading 很大但給分不會很糟的課。

### 太極拳初級
成績：B-
隨便亂選的體育，原本想說太極拳感覺蠻酷的，但是給人的感覺就是舞蹈課，整學期只有錄影、一份心得跟期末考，期末考就是要把完整教過的拳打過一遍，錄影就是要錄下自己打完一套拳的影片。我學期中開始基本上就都第二個小時才到，但是下課才點名所以好像還好，而心得有好好寫，期末考和錄影前我還花了整個周末打拳，從零開始（因為我上課都很晚才到）學，但是我自己覺得我最後其實練得還蠻好的(?，心得是加分用的我也好好寫，結果最後還是吃了 B-，完全搞不懂，後來聽其他同學說這門課是老師看心情給分，然後我被重擊了，所以我大不推這門課。
但其實這門課的這個助教很認真，第一次看到體育課還有開 TA hour 的，我也曾經去 TA hour 一兩次把基礎打好，但是游添燈老師的給分實在是讓人難以接受。

### 深造預備英文寫作與口語表達
成績：A
整學期第二喜歡的課，會先講學術論文的寫作該注意什麼，接著講怎麼寫 Resume/CV，再來是 SOP/POS。作業就是要寫一份 Resume/CV 和 SOP/POS（視目標學校而定），接著會繼續講學術論文，最後講 Academic Presentation 和 slide preparation 要注意的東西。有期中考和期末報告，期中考就是考學術寫作的注意點，期末報告則是老師給了好幾篇經濟系相關的 paper（因為這是經濟系開的課），每組要挑一篇讀完後要 present 給大家。但老師會一步一步的先要求大家寫 outline，接著寫 script，每一步都會給建議，所以不會那麼的沒有頭緒。其實這堂課應該是預設大家都已經有了目標科系，在準備申請國外大學，可是這部分沒有寫在課程說明裡面，導致我其實連有沒有要出國留學都還不知道的情況下，我只好隨便先選了一個學校。老師也不會因為我才二年級就不理，她給了其他人的申請建議，也都有好好的跟我提醒這間學校根據以往經驗可能會需要注意什麼，所以我其實越聽越覺得心虛 XD。這門課不是通識，而是經濟系的選修，但不知道是我剛好修到了特別認真的老師，還是說其實資工系以外的課的老師都很認真，就連資工系被說很認真教學的蕭旭君老師我覺得都比不上這個老師。非常推薦大家來修，不過還是比較建議大三或大四已經準備要出國了再來。
成績的部分只能說不會給很低，但是 loading 不小而且要 A+ 似乎很難，我覺得我其實用了很多心思在這堂課了但還是只有 A，也可能是英文寫作類的東西我本來就很不擅長吧。

### 日文二下
成績：停修
超好笑，N1 在日文二下停修。
期中考不知道為啥考了個 79 分，算下來要 A+ 似乎期末要很高分，其實我覺得我好好讀也可以，只是因為老師在下學期時突然跟大家說這學期的期末要拍小組短劇，然後我在分組的時候沒有抓機會找到那些看起來很認真的，導致組員都是那種看起來又社恐又混混的，考慮到期末短劇的成績也很會影響我的成績（因為期中考），而且覺得跟這群人共事體驗只會很差，所以期中考發考卷的當天我就衝回系館拿停修單給老師簽名了。

# 課外
## JLPT N1
這學期的大東西應該就是 N1 拿了及格！雖然是壓線就是了。原本想說 N1 應該得好好準備，先買了幾回考古題，想說寫完了有空再買參考書，結果上學期因為課業 loading 太大導致連考古題都一題沒寫就上場了。聽力都聽不太懂，因為平常也沒有什麼聽日文的習慣。但因為平常還算看不少日文，所以閱讀跟文法就還不錯，而單字的部分因為實在是有很多日常見不到的單字所以其實蠻糟的（但沒有聽力糟）。最後也是幸好有壓線通過，108/180 之類的，及格線是 100。
我現在終於有資格說 N1 其實真的沒什麼了，我考過 N1 了之後還是去日本玩的時候跟店員講話都很吃力。不過可能也還是有種信心加成(?)，在走出新手村之後我最近開始比較敢在 DC 語音頻道之類的跟日本人講話，其實我覺得我最近因為講話的日文能力的提升比我之前都還要多，果然實際運用才是正確的。

## SITCON 年會
當了 2024 SITCON 的議程組，議程組實在是很忙，而且我又負責 Keynote speaker 和學生講者的聯絡，導致一二月的時候一直在寄信寄信。然後邀請 Keynote 講者邀請了好幾個都沒有實在是很可怕，年會前要確認各種事情也是很可怕，幸好我當初只接了小組員，不然我可能會直接爆炸。

## SITCON Hackathon
SITCON Hackathon 是今年第一次辦的東西，所以很多事情要從零開始想，而我是接了資訊組的組長，主要是負責官網等各種網頁的開發。當時網頁要上線的日子剛好在年會後不久，所以我年會後的那一兩個禮拜幾乎每天有空的時間都花在寫 code，大爆肝的結果是網站的呈現感覺還不錯，這部分也很感謝組員們很給力！
官網：https://hackathon.sitcon.org/2024/

# 後言
因為上學期真的太爆肝了，這學期原本想說接很少活動和修很少課，所以這學期其實系外的課比系上的課還要多，但不知道為什麼 loading 還是爆炸了。
寫這篇文也想訓誡自己暑假要好好上進，不要整天打 LOL 打到人沒了。
對下學期甚至之後的生活還在迷惘，希望能找到方向。