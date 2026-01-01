#MINI PROJECT

CODE:
from datetime import datetime
name=input("enter name:")
lists='''
rice    rs 20/kg
Sugar   rs 30/kg
salt    rs 20/kg
oil     rs 80/liter
paneer  rs 110/kg
maggi   rs 40/each
boost   rs 80/each
colgate rs 85/each
'''
price=0
pricelist=[]
totalprice=0
finalprice=0
ilist=[]
qlist=[]
plist=[]
items={'rice':20,'sugar':30,'salt':20,'oil':80,'paneer':110,'maggi':40,'colgate':85,'boost':80}
option=int(input("for list items press 1"))
if option==1:
    print(lists)
for i in range(len(items)):
    inp1=int(input("if you want to buy press1 and 2 for exit"))    
    if inp1==2:
        break
    elif inp1==1:
        item=input("enter your items:")
        quantity=int(input("enter quantity:"))    
        if item in items.keys():
            price=quantity*(items[item])
            pricelist.append((item,quantity,items,price))      
            totalprice+=price
            ilist.append(item)
            qlist.append(quantity)
            plist.append(price)
            gst=(totalprice*5)/100
            finalamount=gst+totalprice
        else:
            print("sorry! you entered item is not available")
    else:
        print("you entered wrong number")
    inp=input("can i bill the items or not:")
    if inp=='yes':
        pass
        if finalamount!=0:
            print(25*"=","bhavana supermarket",25*"=")
            print("Name:",name,30*" ","Date:",datetime.now())
            print(75*"-")
            print("sno",8*" ",'items',8*" ",'Quantity',3*" ",'Price')
            for i in range(len(pricelist)):
                print(i,8*' ',5*' ',ilist[i],3*' ',qlist[i],8*" " ,plist[i])
            print(75*"-")
            print(50*" ",'TotalAmount:','Rs',totalprice)
            print("gst amount",40*" ",'Rs',gst) 
            print(75*"-")
            print(50*" ",'finalAmount','Rs',finalamount)
            print(75*"-")
            print(20*" ","thanks for visiting")
            print(75*"-")

output:
https://github.com/user-attachments/assets/e776d83a-ee99-4f9a-b538-4db110c9e8e2
