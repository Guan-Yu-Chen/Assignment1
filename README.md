# Assignment1
Assignment1 主要目的是紀錄「計算機概論」這門課的每週作業，使用的語言是C++。

前面幾週的作業偏向基礎練習，我個人認為比較有趣、令我印象深刻的是Week10、Week13和Week15的作業。這三週的作業讓我們使用蒙地卡羅法來解決問題。

## Week10
**Monty Hall Problem（三門問題）**，換門與不換門，哪個策略中獎的機率比較高？  
其實我第一次聽到這個問題時，直覺判斷也認為是1/2的機率。但事實上，換門的話，中獎機率是2/3，而不換的話則是1/3。用蒙地卡羅法去模擬的話也會得到和1/3、2/3接近的數據。  

<img src="https://i.imgur.com/YTYQ1Lm.png" width="60%">

## Week13
**計算π**，一個非常經典的蒙地卡羅法的應用。  
這裡我用的方法是隨機在單位正方形裡產生點，再計算這些點距離原點的距離，判斷是不是在四分之一圓內，以範圍內點的數量作為面積，最後再用
`(1×1×π)/(1×1) = (四分之一圓面積)/(單位正方形面積)` 這條公式，就可以計算出接近π的數值。  

<img src="https://i.imgur.com/poZcaff.png" width="60%">

<img src="https://i.imgur.com/pqhVXLi.png" width="60%">

產生的點越多，計算出來的值就越接近pi。

## Week15
這週的作業出自一則新聞，大致如下：  

> 台灣知名實況主丁特在手遊《天堂M》花費400多萬台幣製作遊戲道具，
> 
> 471次中僅成功11次，遠遠小於官方提供的機率10%，因此決定向遊戲公司提告。

這次作業用蒙地卡羅法模擬1000萬個玩家和製作471次遊戲道具，統計並計算出有多少玩家和丁特一樣只做出11個道具

<img src="https://i.imgur.com/SxcANY0.png" width="60%">

從模擬出來的數據可以看出，在機率是10%的情況下，只製作出不到20個道具的機率是千萬分之29，而像丁特一樣只製作出11個道具的機率甚至低於千萬分之一。基本上已經可以認定官方提供的10%機率是不合理的了。
