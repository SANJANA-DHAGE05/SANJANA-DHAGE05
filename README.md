def AddQ(queue):
    item= input("ENTER ELE:")
    queue.append(item)
    print("item:"+item+"added.")
print()
def DelQ(queue):
    if len(queue)==0:
        print("Q Empty")
    else:
        item=queue.pop(0)
        print("item:"+item+"deleted.")
print()
def DispQ(queue):
    if len(queue)==0:
        print("Q Empty")
        return          
    print("THE ELEMENTS ARE:  ")
    for item in queue:
        print(item)
print()
def main():
    queue=[]
    while True:
        choice=int(input("ENTER 1.ADD 2. DEL 3,DISP 4.EXIT"))
        print()

        if (choice==1):
            AddQ(queue)
        elif (choice==2):
            DelQ(queue)
        elif (choice==3):
            DispQ(queue)
        else:
            print("end")
            print()
            break


print()
if __name__=="__main__":
    main()


