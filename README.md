# -Python-Project-10
#10 Combining names

print("Hello! Nice to meet you :)\n")

def main():

    user_city = input("In which city do you grew up?\n").capitalize()
    print (f"I never was in {user_city} before!")

    user_pet = input("Hey ! What\'s the name of your pet?\n").capitalize()
    print(f"That\'s a cool name for a pet! {user_pet} sounds nice.\n")

    print(f"So i name you... {user_city} {user_pet}")

    def yes_no(message):
        userinput = str(input(message)).lower()
        if userinput == "yes":
            return 1
        elif userinput == "no":
            return 0
        else:
            return yes_no("Please, use 'yes' or 'no'.\n")

    answer = yes_no("Do you want to try again?\n")
    if answer == 1:
        print("Yeah ! Let\'s do another one!\n")
        main()
    elif answer == 0:
        print(f"Goodbye {user_city} {user_pet} ! Take care :)")

main()
