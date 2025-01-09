# assignmentP
cheatsheet+课程资料和情报

# 计概B上机 Cheatsheet

print(f'{c} {b}')：输出计算后的答案（鸡兔同笼）

p[i]>=p[k-1]：每个i项与k项比较（next round）

a=input().lower()：小写字母（petya and strings）

a=input().upper()：大写字母（petya and strings）

ord(a[i])==ord(b[i])：将字母转换成数字比较大小（petya and strings）

dp=[0]*26：dp做法，创造26个单位的0（boy or girl）

a=[0]*26
for i in q:
a[ord(i)-ord('a')]+=1：证明dp的项也有位置之分，从0开始到n-1（boy or girl）

for i in range(len(colour)-1)：因为比较次数会少一次，所以需要-1防止爆表（stones on the table）

for i in range(5):
    n=list(map(int,input().split()))
for j in range(5):：i是横的，j是竖的（beautiful matrix）

if n[j]==1:
total_step=abs(i-2)+abs(j-2)：abs保持正整数（beautiful matrix）

money_map=[
    100,20,10,5,1
]：列表法，方便按顺序查找对比（hit the lottery）

result=[]：创建空列表，方便储存数据（sum of round numbers）

n.remove(max(n))：从列表中移除（restoring three numbers）

number[0]+number[1]==x：证明列表中有位置之分，从0开始到n-1（sum）

print(''.join(letter))：让分开的元素在输出时贴在一起（word capitalization）

number=[i%2 for i in number]：一边进行计算一边加入列表（IQ test）

print(number.index(1)+1)：index索引位置，列表从0开始，+1防止输出错位（IQ test）

v=[(weather[i],i) for i in range(n)]：将另一个列表中的元素照抄，并加入了每个元素的索引位置（restore the weather）

v.sort()：将列表中的元素按照顺序排列（restore the weather）

z[v[i][1]]=real[i]：将v的i项的第1个元素（从0开始）索引位置，将real 的数据添加至z列表中（restore the weather）

tmp=L[0]+' '：证明普通的input也是有位置之分，从0开始到n-1（06374 文字排版）

ans.append()：在列表中添加（06374 文字排版）

ans.append(tmp.rstrip())：列表右边保留没有东西（06374 文字排版）

print('\n'.join(ans))：在列表的每个元素间添加空行（06374文字排版）

list.append('('+n[i]+','+str(count)+')')：在仍在处理中的列表加入固定的格式以及计算好的数据（后续还可能添加其他的数据）（‘(‘以及+n[i]+）（12556编码字符串）

for j in range(s,e+1):：由于范围的最后一个数字都不会被纳入，因此需要+1调整（02808校门外的树）

print(dp.count(1))：计算数目（02808校门外的树）

ans+=input().replace('### ###','').count('###')//2：将原本的字符替换成另一个字符（19949提取实体）

21532数学密码（数学思维个例）

for e in [a,-a]:：给元素赋值两个数值（18223 24点）

flag=False：给反馈（18223 24点）

flag=True：给反馈（18223 24点）

i=float(input())：输入时需要保留浮点数（01003 hangover）

Multiply by 2, divide by 6（数学思维个例）

def zhishuhanshu(n):
    from math import sqrt
    zhishu,shangxian=[],int(sqrt(n))+1
    for i in range(2,shangxian):
        while n%i==0:
            zhishu.append(i)
            n/=i
    if n>1:
        zhishu.append(n)

return zhishu：找一个数字里面的质因数（23564 数论）

set_zhishu=len(set(zhishu))：set中会避免重复的数据（23564 数论）

# 课程资料和情报
闫老师的课主要都是需要靠自己自学编程，以及课堂上也会抽一些题目以及一些编程方法进行概念讲解，而且还可以自行选择学习C++或是python。此外，每周需要提交的功课为6题编程题，以及每天都会给2道每日选做（后期为每日1道）。每个月会有一次计概的上机模拟考试，不计分，主要是为了让学生可以熟悉考试环境，还可以对自我进行附有时间限制的编程练习。真的需要多练、多看、多想才能更熟练地编程。

这是每日选做的做题网站：
https://github.com/GMyhf/2024fall-cs101/blob/main/problem_list_at_2024fall.md
