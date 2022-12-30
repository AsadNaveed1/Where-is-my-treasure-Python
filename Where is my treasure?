Treasureinput = input()
lst = []
for o in Treasureinput:
    lst += [o]
trsre = [lst]
for q in range(len(lst) - 1):
    rw = input()
    nlst = []
    for v in rw:
        nlst += [v]
    trsre.append(nlst)


Mapinput = input()
lst2 = []
for a in Mapinput:
    lst2 += [a]
MPofTrsre = [lst2]
for j in range(len(lst2) - 1):
    rw2 = input()
    nlst2 = []
    for g in rw2:
        nlst2 += [g]
    MPofTrsre.append(nlst2)

def tester():
    lstcheker = -1
    Counter = -1
    x = len(lst2) - (len(lst)) + 1
    for k in MPofTrsre:
        trsresize = 0
        Counter += 1
        test = 1
        Box = 0
        lstcheker += 1
        for t in range(len(lst2)):
            if test <= x and Box <= len(trsre):
                if trsre[trsresize] == k[t:(t + len(lst))]:
                    trsresize = 1
                    Box += 1
                    pole = True
                    while pole == True:
                        if (len(lst) + (lstcheker + 1)) <= len(lst2) + 1:
                            if trsre[trsresize] == MPofTrsre[lstcheker + trsresize][t:(t + len(lst))]:
                                trsresize += 1
                                if trsresize == len(lst):
                                    print(t, Counter)
                                    return True

                            else:
                                trsresize = 0
                                pole = False
                        else:
                            pole = False
                else:
                    test += 1

    return False


import sys
game = False
if game == False:
    if tester() ==  True:
        sys.exit()



trsre = trsre[::-1]
for d in range(len(trsre)):
    for u in range(d):
        if d != u:
            trsre[d][u], trsre[u][d] = trsre[u][d], trsre[d][u]

game = False
if game == False:
    if tester() == True:
        sys.exit()


trsre = trsre[::-1]
for d in range(len(trsre)):
    for u in range(d):
        if d != u:
            trsre[d][u], trsre[u][d] = trsre[u][d], trsre[d][u]

game = False
if game == False:
    if tester() == True:
        sys.exit()

trsre = trsre[::-1]
for d in range(len(trsre)):
    for u in range(d):
        if d != u:
            trsre[d][u], trsre[u][d] = trsre[u][d], trsre[d][u]

game = False
if game == False:
    if tester() == True:
        sys.exit()
