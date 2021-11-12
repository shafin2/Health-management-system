# Health-management-system
def getdate():
    import datetime
    return datetime.datetime.now()
date=getdate()
def exercise():
    date = getdate()
    print("Now date/time is",date,"\nEnter the Exercise")
    exer = input()
    f.write("\n")
    f.write(str(date))
    f.write("\n")
    f.write(exer)
    f.close()
def diet():
    date = getdate()
    print("Now date/time is",date,"\nEnter the Diet")
    diet = input()
    f.write("\n")
    f.write(str(date))
    f.write("\n")
    f.write(diet)
    f.close()

while(True):
    print("Welcome to health management system")
    print("In that system you can add both diet and exercise for Ali,Shafin and Robot")
    print("So press 1 for Ali,2 for shafin and 3 for robot")
    client_name = int(input())
    if client_name == 1:
        print("Press 1 for Ali's exercise and 2 for Ali's diet")
        choice = int(input())
        if choice == 1:
            f = open("AliExercise.txt", "a")
            exercise()
        elif choice == 2:
            f = open("AliDiet.txt", "a")
            diet()
        else:
            print("Sorry,You did not enter the write number Try Again")
            continue
        break
    elif client_name == 2:
        print("Press 1 for Shafin's exercise and 2 for Shafin's diet")
        choice = int(input())
        if choice == 1:
            f = open("ShafinExercise.txt", "a")
            exercise()
        elif choice == 2:
            f = open("ShafinDiet.txt", "a")
            diet()
        else:
            print("Sorry,You did not enter the write number Try Agian")
            continue
        break
    elif client_name == 3:
        print("Press 1 for Robot's exercise and 2 for Robots's diet")
        choice = int(input())
        if choice == 1:
            f = open("RobotExercise.txt", "a")
            exercise()
        elif choice == 2:
            f = open("RobotDiet.txt", "a")
            diet()
        else:
            print("Sorru,You did not enter the write number Try again")
            continue
        break

    else:
        print("Sorry you did not choose right number\nyou have to choose 1,2,3 for Ali,Shafin and Robot")
        print("Try Again")
        continue
print("Your entered data is safe Byeeee")

