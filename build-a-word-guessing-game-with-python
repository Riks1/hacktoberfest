import random

wordList = ["rizz", "ohio", "sigma", "tiktok", "skibidi","tree", "book", "game", "fish", "road",        
    "apple", "grape", "melon", "berry", "lemon", 
    "orange", "banana", "friend", "circle", "planet",  
    "train", "cloud", "stars", "light", "snake"  
]

word = random.choice(wordList)
def get_feedback(guess, word):
    feedback = []
    for i in range(len(guess)):
        if guess[i] == word[i]:
            feedback.append("🟩")  
        elif guess[i] in word:
            feedback.append("🟨")  
        else:
            feedback.append("⬜")  
    return "".join(feedback)

guessedWord = ['_'] * len(word)

attempts = 6

while attempts > 0:
   
    print("\nCurrent word: " + ' '.join(guessedWord))

    guess = input("Guess the word: ").lower()
   
    if guess not in word:
        print('Not exactly!')
        
    feedback = get_feedback(guess,word)
    print(feedback)
    if guess == word:
      print('Congrats! You guessed the word!')
      break
    attempts -= 1
else:
    print("\nYou've run out of attempts! The word was: " + word)
