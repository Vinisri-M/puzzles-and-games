import random
def guessnum(n):
    randomnum=random.randint(1,n)
    guessnum=0
    while(guessnum!=randomnum):
        guessnum=int(input(f'Guess a number between 1 and {n}:'))
        if guessnum<randomnum:
            print("your guess is very low,.Try again.")
        elif guessnum>randomnum:
            print("your guess is very high.Try again.")
    print(f"Hurrah,you have guessed the number {randomnum} correctly.")
guessnum(10)
