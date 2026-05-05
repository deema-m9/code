# code
my mini project
Sephora store invoice including tax and discount
python
print , int , float , input , Variables , if , elif , else
print("Welcome to Sephora")
def stor():
    product=input("Enter the product name: ")
    quantity=int(input("How many products did you buy? "))
    price=float(input("Enter the price of the product: "))
    total=price*quantity
    print("The total price is:",total)
    tax=total*0.15
    print("The tax is:",tax)
    final_total=total+tax
    print("the final total: ", final_total)
    if quantity >= 10 :
        discount = final_total * 0.29
        final_total = final_total - discount
        print("You have a dispute 29%")
    elif quantity >= 5 :
        discount = final_total * 0.05
        final_total = final_total - discount
        print("You have a dispute 5%")
    else:
        print("You don't have a dispute")
    print("The final total after discount is:", final_total)
stor()
