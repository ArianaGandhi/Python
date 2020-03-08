name = input("Enter file:")
if len(name) < 1 : name = "mbox-short.txt"
lines = open(name)
l=list()
dic=dict()
for line in lines:
    line.strip()
    if line.startswith('From: '):
        l=line.split() 
        if l[1] not in dic:
            dic.update({l[1]:1})
        else:
            dic[l[1]]=dic[l[1]]+1
maxcount=0
maxname=str()
for key,val in dic.items():
    if val>maxcount:
        maxcount=val
        maxname=key
print(maxname,maxcount)
