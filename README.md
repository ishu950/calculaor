# calculaor
project3



def calculator():
    num1 = float(input("whats ther first num: "))
    num2 = float(input("whats ther sec num: "))

    list = ["+", "-", "*", "%"]
    print(list)
    op = input("choose any perator ")

    any_op = False
    while  not any_op:

            if op == "+":
                num3=num1+num2
                print(num3)

            elif op=="-":
                num3=num1-num2
                print(num3)

            elif op == "*":
                num3=num1*num2
                print(num3)
            elif op=="%":
                num3=num1%num3
                print(num3)


            ask_cont=input("whter wnna continue or stop? yes or no ")
            if ask_cont=="no":
                any_op=True
                print(f"ans is {num3}")
            else:
                any_op=False
                num1=num3
                num2=float(input(" num2"))
                op = input("choose any perator ")
                print(num3)




calculator()
