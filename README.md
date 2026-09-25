print("================================================")
print("           PERSONAL HYGIENE HEALTHCARE          ")
print("================================================")

print("PRODUCT MENU")
print("[S] SHAMPOO                  -15")
print("[C] CLOSEUP                  -35")
print("[D] DOVE SOAP                -150")
print("[B] BODYOIL                  -90")
print("================================================")
print("                    RECIEPT       ")
print("================================================")

code = input("Enter product code: ").upper()

if code == "S":
    product = "SHAMPOO"
    price = 15
    print(f"Product price :P{price:.2f}")
    qty = int(input("Enter Quantity: "))
elif code == "C":
    product = "CLOSEUP"
    price = 35
    print(f"Product price :P{price:.2f}")
    qty = int(input("Enter Quantity: "))
elif code == "D":
    product = "DOVE SOAP"
    price = 150
    print(f"Product price :P{price:.2f}")
    qty = int(input("Enter Quantity: "))
elif code == "B":
    product = "BODYOIL"
    price = 90
    print(f"Product price :P{price:.2f}")
    qty = int(input("Enter Quantity: "))
else:
    print("INVALID CODE")
    exit()

total = price * qty
print(f"Total             :P{total:.2f}")


add_more = input("Add another product? (Y/N): ").upper()
if add_more == "Y":
   print("PRODUCT MENU")
   print("[S] SHAMPOO                  -15")
   print("[C] CLOSEUP                  -35")
   print("[D] DOVE SOAP                -150")
   print("[B] BODYOIL                  -90")
   choice = input("Add another product code:  ").upper()
   print(f"2nd product       :{choice}")
   if choice == "S":
        product = "SHAMPOO"
        p = 15
        print(f"2nd product price :P{p}")
        qty = int(input("Enter Quantity: "))
        tot = p * qty
        print(f"Total             :P{tot:.2f}")
   elif choice == "C":
        product = "CLOSEUP"
        p = 35
        print(f"2nd product price :P{p}")
        qty = int(input("Enter Quantity: "))
        tot = p * qty
        print(f"Total             :P{tot:.2f}")
   elif choice == "D":
        product = "DOVE SOAP"
        p = 150
        print(f"2nd product price :P{p}")
        qty = int(input("Enter Quantity: "))
        tot = p * qty
        print(f"Total             :P{tot:.2f}")
   elif choice == "B":
        product = "BODYOIL"
        p= 90
        print(f"2nd product price :P{p}")
        qty = int(input("Enter Quantity: "))
        tot = p * qty
        print(f"Total             :P{tot:.2f}")
else:
   print("NO ADDED ITEM")

subtotal = total + tot
discount_rate = float(input("Enter DISCOUNT (%): "))
discount = subtotal * (discount_rate/100)
discount_amt = subtotal - discount
tax = discount_amt * 0.12
final_total = discount_amt + tax
print("================================================")
print(f"Subtotal          :P{subtotal:.2f}")
print(f"Discount          :P{discount:.2f}")
print(f"Discount_amt      :P{discount_amt:.2f}")
print(f"Tax               :P{tax:.2f}")
print(f"Final Total       :P{final_total:.2f}")
print("================================================")

payment = float(input("Enter Payment  : P"))

if payment >= final_total:
    change = payment - final_total
    print(f"Payment        :P{payment:.2f}")
    print(f"Change         :P{change:.2f}")
else:
    balance = final_total - payment
    print("Insufficient Payment!")
    print(f"Balance        :P{balance:.2f}")

print("================================================")
print("   THANK YOU FOR YOUR VALUED TRUST AND CONTINUED SUPPORT!    ")
print("================================================")
