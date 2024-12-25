## 11328201 學習歷程
** C語言與python的條件式

C：
scanf("%d", &score);
if(score>=90){
    printf("A");
}
else if(score>=80)
......

python：
```python
score=int(input())
if score>=90:
    print("A");
elif score>=80:
......
```

** python的迴圈式
while 條件(條件成立時):重複到不符合條件時，break
for i in range(a, b):重複b-a次，i=a、i=a+1...i=b-1

```python
n=int(input())
i=1
while i<n+1:
    for j in range(1, i+1):
        print("*"*j)
    i=i+1
```

tasks = [
    {"title": "寫報告", "description": "完成期末專案報告", "due_date": "2025-01-14", "priority": "高", "completed": False},
    {"title": "期末考", "description": "複習已學", "test_date":"1/7~1/10", "priority": "中", "completed": False},
]
\\描述任務清單中的各種名稱和各項資料
