# guessing-a-number-game-in-python
using python to guess a number
// Given python code
flag=0
print("Guess the number !!",end=" ")

while(True):
    var = int(input())
    if var>18:
        print("Guess a smaller number")
        flag=flag+1
        print("Number of guesses left",end=" ")
        print(9-flag)
    if var<18:
        print("Guess a bigger number")
        flag=flag+1
        print("Number of guesses left",end=" ")
        print(9-flag)
    if var==18:
        print("You won the game!!")
        print("The number of guesses you took:",flag)
        break
    if flag==9:
        print("You lost the game!!!")
        break

