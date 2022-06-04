import random
R = "Rock"
P = "Paper"
S = "Scissors"

while True:
    Player = input("Enter a choice (R, P, S): ")
    possible_actions = ["R", "P", "S"]
    CPU = random.choice(possible_actions)
    print(f"\nYou chose {Player}, computer chose {CPU}.\n")

    if Player == CPU:
        print(f"Both players selected {Player}. It's a tie!")

    elif Player == "R":
        if CPU == "S":
            print("Rock beats scissors! You win!")
        else:
            print("Paper beats rock! CPU wins.")
    elif Player == "P":
        if CPU == "R":
            print("Paper beats rock! You win!")
        else:
            print("Scissors beats paper! CPU wins.")
    elif Player == "S":
        if CPU == "P":
            print("Scissors beats paper! You win!")
        else:
            print("Rock beats scissors! CPU wins.")

        break
