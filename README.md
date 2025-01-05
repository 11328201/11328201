## 11328201 學習歷程
**條件式


C：
scanf("%d", &score);
if(score>=90){
    printf("A");
}
else if(score>=80)
......

python：
程式碼1
```python
score=int(input())
if score>=90:
    print("A");
elif score>=80:
```
......
程式碼2
```python
a=int(input())
if a>=0 and a<=12:
    print("兒童")
elif a>=13 and a<=19:
    print("青少年")
elif a>=20 and a<=64:
    print("成年人")
elif a>=65 and a<=141:
    print("老年人")
else:
    print("請輸入正確年齡")
```
程式碼3
```python
n=int(input())
for j in range(1, n+1):
    print("*"*j)
```
程式碼4
```python
n=int(input())
i=1
while i<=n:
    print("*"*i)
    i=i+1
```
程式碼5
```python
def f(n):
    return n**2+5*n+4
a=int(input())
print(f(a))
```
程式碼6
```python
def f(n):
    k=0
    a=n**0.5
    for i in range(2, a+1):
        if n%i==0:
            k=k+1
    if k=0:
        return 1 #是質數
    else:
        return 0 #不是質數
sum=0
M, N=int(split().input())
for j in range(M, N+1):
    if f(j)=1:
        sum=sum+j
print(sum)
```
程式碼7
```python
def f(n):
    if n==0 or n==1:
        return 1
    elif n==2:
        return 2
    else:
        return f(n-3)+f(n-2)+f(n-1)
N=int(input())
print(f(N))
```

程式碼8
```python
a=[3, 4, 5, 6]
a[2]=9
print(a)
```
輸出結果為：[3, 4, 9, 6]
程式碼9
```python
a=(3, 4, 5, 6)
a[2]=9
print(a)
```
無法正確輸出
程式碼10
```python
a={3, 4, 3, 5, 6}
print(a)
```
輸出結果為：{3, 4, 5, 6}
程式碼11
```python
dic={
    "A"="a",
    "B"="b",
    "C"="c",
}
print(dic)
print("C" in dic)
print("D" in dic)
C=dic.pop("C")
print(C)
print(dic)
```
print("C" in dic)中，字典裡有"C"這個元素，所以輸出True
print("D" in dic)中，字典裡沒有"D"這個元素，所以輸出False
C=dic.pop("C")可將元素"C"儲存到變數C中，元素"C"被提取出來
print(C) 的輸出為c
print(dic) 的輸出變成{
    "A"="a", "B"="b"}

實作遊戲：條件式應用、while迴圈應用
程式碼12
```python
k=1;
while k==1:
    print("情境：你是一名美國留學生，你的室友這天晚上8:00說他要和他的朋友在特定地點交易，車程需要30分鐘，他希望你開車載他。")
    print("(1) \"為什麼地點那麼遠？\"")
    print("(2) \"好，我剛好有空。\"")
    print("(3) 查找地圖資料，確認當地安全性")
    a=int(input())
    if a==1:
        print("他說：\"我和他一樣都不會開車\"，你接著開車和他前往當地。")
    elif a==2:
        print("你接著開車和他前往當地。")
    elif a==3:
        print("你查到當地不良分子經常出沒，並且保安設施比較不完善，接著你追問室友，發現他太執著於利益差點帶著你一起踏入危險。")
        print("最後，你室友所說的\"朋友\"其實是個你室友不認識的搶劫慣犯，你成功化險為夷。")
        print("你的分數:100")
        break
    print("到達目的地後，發現這裡蠻偏遠的，而且天空很昏暗，看起來有點可怕，你們來到一處除了一家便利商店，四周幾乎沒有建築物的地方")
    print("然後在不遠處看到一個身高大約190公分的男子，室友接著拉下窗戶和他認親，他說覺得在這裡交易很奇怪，想換個地方。")
    print("他想上你們的車，然後你的室友直接幫他打開了車門鎖。")
    print("在開車的路上你們和這名男子聊了一會，聊到他是大學幾年級的時候，他突然說：\"我不是大學生，而是搶劫犯，你們現在被搶了。\"")
    print("起初你還以為這是玩笑，但他接著將一把短刀抵在你的腰旁邊。距離搶劫犯所說的目的地還有點距離，且不知為何，路上碰到很多警車。")
    print("等紅綠燈時，身邊圍繞著警車，正當你在猶豫時，搶劫犯拿著刀輕聲說：\"別做傻事\"。")
    print("(1) 靜靜的聽從搶劫犯的指示")
    print("(2) 打開車門向外逃出")
    print("(3) 拉下窗戶大聲求救")
    b=int(input())
    if b==1:
        print("你們默默的經過很多警車，來到了搶劫犯指定的目的地。")
    elif b==2 or b==3:
        print("犯人驚慌失措，失手將刀刺入你的內臟器官，雖然搶劫犯被迅速逮捕，但你的性命也迎來了結束。")
        print("你的分數:0")
        break
    print("你們來到的地方是個小型停車場，前面有一個藥局，搶劫犯叫你去提款機領1000元，你和他說你只有200元。")
    print("他說那種事他才不管，給我領1000元就對了，你害怕的走向提款機，把卡裡的200元領了出來，接著準備回車上時。")
    print("你被當成人質的室友從車裡逃了出來，然後大聲和你說：\"快跑、跑\"。搶劫犯以飛快的腳步追著你的室友，接下來...")
    print("(1) 你向藥局逃跑")
    print("(2) 和室友利用人數優勢試圖壓制他")
    print("(3) 向車子方向跑，試圖拿下車然後用車子壓制他")
    c=int(input())
    if c==2:
        print("你們雖然有兩個人，但在刀子面前還是抵制不住，最後犯人將你們滅口並逃生")
        print("你的分數:0")
        break
    elif c==3:
        print("你試圖跑回車子，但他以驚人的跑步速度向你前來，接著在你一上車還來不及 關上車門，他就抵住車門。")
        print("他慌張地用刀刺向坐在駕駛座的你，此時你的右胸口被刺入...")
        print("(1) 喊出聲，露出痛苦的表情")
        print("(2) 默默的一言不發，忍耐痛楚")
        print("(3) 將刀拔出，並用來壓制他")
        d=int(input())
        if d==1 or d==2:
            print("他雖然慌了，但點到為止，將你甩下車，接著開著你的車子逃逸")
        elif d==3:
            print("你用刀傷到了他，但因為出血過多，你的性命迎來了結束")
            print("註：被刀刺入時，強行拔出容易大量出血")
            print("你的分數:0")
            k=0
            break
        print("接著你在藥局護士的急救，和而後趕來的救護車下，成功保住性命。")
        print("註：逃跑三順序是跑躲打，跑是第一優先，接著找地方躲起來，真的躲不掉時才打，但\"打\"的禁忌是肉搏。")
        print("身邊所有物品都可以拿來當作武器，唯獨不能用肉身打。")
        print("你的分數:70")
        break
    elif c==1:
        print("你和藥局裡的人描述了一下外面發生的狀況，藥局裡的人立刻叫了警車來，接著他開著你的車子逃逸。")
        print("你的分數:90")
        break
```