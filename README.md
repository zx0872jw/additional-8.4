# additional-8.4
# write def main(): ... on line 3

    grocery_list = {}
    grocery_1 = str(input("Enter grocery item 1: "))
    price_1 = int(input("Enter price item 1: "))
    grocery_2 = str(input("Enter grocery item 2: "))
    price_2 = int(input("Enter price item 2: "))
    grocery_3 = str(input("Enter grocery item 3: "))
    price_3 = int(input("Enter price item 3: "))
    
    grocery_list[grocery_1] = price_1
    grocery_list[grocery_2] = price_2
    grocery_list[grocery_3] = price_3
    
    for grocery, price in grocery_list.items():
        print("Grocery: %s, Price: $%0.2f" %(grocery, price))
        
    grocery_4 = str(input("Enter grocery item 4: "))
    price_4 = int(input("Enter price of item 4: "))
    
    grocery_list[grocery_4] = price_4
    
    delete_grocery = str(input("Enter one of your grocery items: "))
    del grocery_list[delete_grocery]
    for grocery, price in grocery_list.items():
        print("Grocery: %s, Price: $%0.2f" %(grocery, price))
        
main()
