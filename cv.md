
# Bal Artsemi
---
1. **Contact:**
    - *G-mail:* blackpawsstudio@gmail.com;
    - [*VK*](https://vk.com/id224429894); 
    - *Discord:* Артемий Баль #6126;
---
2. **Objective:**
> Learn how to be frontend developer. I want to face some difficult problems on this course, solve them, get new information about frontend and JavaScript development;  
---
3. **Programming experience:**
    Some layout in HTML/CSS;
    Solving some problems in JavaScript on Codewars;
    Backend in Python;
    Studied C# and Delphi in college;
---
4. **Code sample in Python:**
```
def data_input():
    f= open ('data2.txt')
    dot = []
    for line in f:
        dot.append(line)
    for el in dot:
        st = el.split()
        i = 0
        while i < len(st):
            st[i] = int(st[i])
            i+=1
        dotlist.append(st)

def final_point(fin):
    i = 0
    for el in dotlist:
        if fin<el[1]:
            fin = el [1]
    return  fin

def find_path():
    currdot = [0]
    notice = False
    j=0
    k = 0
    while int(currdot[j]) < (len(dotlist)/2):
        i = 0
    while i < (len(dotlist)):
        if dotlist[i][2] != 0 and dotlist[i][0] in currdot:
            path.append(dotlist[i])
            currdot.append(path[k][1])
            k+=1
            if dotlist[i][1]==final:
                notice = True
                break
        i += 1 
        if notice:
            break
        j+=1
        if j>100:
            notice = True
            break
                            
def cleanlist(arr):
    M = []
    for e in arr:
        if e in M:
            continue
        M.append(e)
    return M

def traceback(arr, v):
    r=[]
    currarc = arr.pop()
    currdot = currarc[1]
    r.append(currarc[2])
    prevdot = currarc[0]
    trace = []
    trace.append(currarc)
    while arr != []:
        currarc = arr.pop()
        currdot = currarc[1]
        if prevdot == currdot:
            trace.append(currarc)
            r.append(currarc[2])
            prevdot = currarc[0]
    r.sort()
    v+=r.pop(0)
    return trace, v

def change_arc(arr,v):
    i=0
    while i<len(arr):
        arr[i][2] = arr[i][2]-v 
        i+=1
    return arr

def check_full(arr):
    for el in arr:
        if el[1] == final:
            return True
        else:
            return False

dotlist = []
path = []
temp = []
v = 0
vmax = 0
final = 0
data_input()
final = (final_point(final))
print('Путь идет из точки 0 в точку', final, '\n')
i=0
try:
    while True:
        i+=1
        find_path()                                
        path = (cleanlist(path))
        temp = traceback(path, v)
        if check_full(temp[0]):
            vmax +=temp[1]
        path = change_arc(temp[0], temp[1])  
        if check_full(temp[0]):
            print('Дуги ', i,' итерации ',path) 
            print('Vmax',vmax,'\n')       
        path = []

        
except IndexError:
        print('Конец работы программы!')
```
---
5. **Working experience:**
    None;
---
6. **Education:**
    - BSUIR filial "MRC";
    - This online cources;
---
7. **Level of English:**
    According to EPAM English test - B1.
