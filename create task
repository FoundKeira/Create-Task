"""REQUIREMENTS"""
#
# use at least one list (that will fulfill the program's purpose)
# allow user to create inputs
# function with a name, definition, one or more parameters, and called
# if and when statement related to my inputs and outputs

#####
"""Global Variables"""
#####

drawerChoice = 0
drawerCount = 3
inventory = []
watch = "Watch set at time 17:38"
note = "Note that says FA1RY"
skullKey = "A key that's handle is molded in the shape of a skull"
key = "A simple key"
chest = "A chest that needs a key"
diary = "Diary dated 10/13/73"
#####
"""helper functions"""
#####
def optionChoice(choice):
    if choice == "1":
        drawerOpen()
    elif choice == "2":
        print("You open the computer.")
        print("As it opens, a title screen appears :")
        print("")
        wifiGuess = input(str("WIFI PASSWORD : "))
        wifiPassword()
    elif choice == "3":
        safeCheck()
    elif choice == "4":
        print(inventory)
        menu()
    elif choice == "5":
        doorCheck()
    elif choice == "6":
        chestCheck()
    else:
        menu()
def menu():
    print("1) Check Cabinet")
    print("2) Check Computer")
    print("3) Check Safe")
    print("4) Check Inventory")
    print("5) Check Door")
    if inventoryCheck(chest) == True:
        print("6) Check Chest")
    choice = input(str("What Would you like to do next?" ))
    optionChoice()


def inventoryCheck(item):
    for i in range (len(inventory)):
        if inventory[i] == item:
            return True
    return False

def inventoryPrint():
    for i in range (len(inventory)):
        print(i + " : " + inventory[i])

def inventoryAdd(item):
    inventory.append(item)
    print(item + " ADDED TO INVENTORY")

def drawerOpen():
    drawerChoice = input(str("There are three drawers. Which one do you open? : "))
    if drawerChoice == "1":
        if inventoryCheck(note) == False:
            print("You find a note in the piles of shirts.")
            print("The note says FA1RY")
            print("")
            inventoryAdd(note)
            print("")
        else:
            print("It is just piles of shirts")
            print("")
    if drawerChoice == "2":
        print("You only spot piles of shirts.")
        print("They are old and have clearly lost their vivid colors and patterns over time.")
        if inventoryCheck(watch) == False:
            print("It is while you search through the shirts that you spot a glimmer of a golden watch.")
            print("The diary was right, the watch reads 17:38.")
            print("")
            inventoryAdd(watch)
            print("")
    if drawerChoice == "3":
        print("You open the third cabinet")
        print("Anticlimactically, this drawer was only filled with pants")
        print("")
    else:
        print("Please enter a number 1-3.")
        drawerOpen()

def wifiPassword(wifiGuess):
    if wifiGuess == str("FA1RY"):
        print("The computer opens on a beautiful valley landscape.")
        print("A screen pops up that reads :")
        print("")
        print("Check under the bed.")
#####
"""Introduction"""
#####

print("You wake up in a room.")
print("The room has a bed, cabinet, computer, a safe, and a door with two locks; one meant for a key, "
      "another that is meant to have an input of four numbers.")
print("You have a book in your lap. As you stretch the spine to open the first page you recognize it is a diary.")
print("")
print("10/13/73")
print("My wife bought me a watch. It keeps getting stuck at the time 17:38 though. I left it in my cabinet to fix another day.")
inventoryAdd(diary)

#####
"""Cabinet"""
#####

drawerOpen()

#####
"""FIRST PUZZLE"""
#####

menu()
