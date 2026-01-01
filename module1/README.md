#MINI PROJECT

from datetime import datetime

name = input("enter name:")

lists = '''
rice rs 20/kg
sugar rs 30/kg
salt rs 20/kg
oil rs 80/liter
paneer rs 110/kg
maggi rs 40/each
boost rs 80/each
colgate rs 85/each
'''

price = 0
pricelist = []
totalprice = 0
finalprice = 0
ilist = []
qlist = []
plist = []

items = {
    'rice': 20,
    'sugar': 30,
    'salt': 20,
    'oil': 80,
    'paneer': 110,
    'maggi': 40,
    'colgate': 85,
    'boost': 80
}

option = int(input("for list items press 1: "))

if option == 1:
    print(lists)

for i in range(len(items)):
    inp1 = int(input("if you want to buy press 1 and 2 for exit: "))

    if inp1 == 2:
        break

    elif inp1 == 1:
        item = input("enter your items: ")
        quantity = int(input("enter quantity: "))

        if item in items.keys():
            price = quantity * items[item]
            pricelist.append((item, quantity, price))
            totalprice += price
            ilist.append(item)
            qlist.append(quantity)
            plist.append(price)

        else:
            print("sorry! you entered item is not available")

    else:
        print("you entered wrong number")

gst = (totalprice * 5) / 100
finalamount = gst + totalprice

inp = input("can i bill the items or not (yes/no): ")

if inp == 'yes' and finalamount != 0:
    print(25 * "=", "Bhavana Supermarket", 25 * "=")
    print("Name:", name, " " * 20, "Date:", datetime.now())
    print(75 * "-")
    print("S.No", "Item", "Quantity", "Price")

    for i in range(len(pricelist)):
        print(i + 1, ilist[i], qlist[i], plist[i])

    print(75 * "-")
    print("Total Amount: Rs", totalprice)
    print("GST Amount: Rs", gst)
    print("Final Amount: Rs", finalamount)
    print(75 * "-")
    print("Thanks for visiting 😊")


output:
![My Screenshot](https://github.com/user-attachments/assets/e776d83a-ee99-4f9a-b538-4db110c9e8e2)
