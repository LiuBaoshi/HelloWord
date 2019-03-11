# HelloWord
This is my first repository

#c15.py解答
#首先定义4级石头价值的算法
def l4_value_compute():
    global l4_value
    l4_value = 0
    num = 1
    global counter
    counter = 0
    while num > rate:
        import random as random
        num = random.random()
        counter += 1
    else:
        l4_value = (l3_value + 16*l1_value + 0.897*gold)*counter + 10*vit
    return l4_value

gold = 1
diamond = 0.05 * gold
vit = gold
rate = 0.4878

l1_value = 0.75*gold + 8*diamond               #先求1个一级石头需要的金币数
l3_value = 13*l1_value + 0.39*gold +10*vit     #再求1个三级石头所需的金币数
l4_value_compute()                             #再求1个四级石头所需的金币数
l6_value = 13*l4_value + 19.75*gold + 10*vit   #求1个六级石头所需的金币数
int_l6_value = int(l6_value) + 1               #不满1的小数进一位成为整型

if l6_value < 750:
    print('自己合成划算')
    # print(l6_value)
    print('此时共花费金币数：' + str(int_l6_value))
    print('四级五行石共合成'+str(counter)+'次')
else:
    print('直接购买划算')
    # print(l6_value)
    print('此时共花费金币数：' + str(int_l6_value))
    print('四级五行石共合成'+str(counter)+'次'
