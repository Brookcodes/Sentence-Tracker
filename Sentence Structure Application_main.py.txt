#Sentence Structure Application
#Ask the user to input the sentence
sentence = input("Enter the sentence: ")
#Count the number of words in the sentence 
words = sentence.split()
print(f"Sentence: {sentence}")
#Display each word in a list format
word_counter = len(words)
for i, word in enumerate(words, start = 1):
    print(f"Word {i}: {word}")
#Find the longest word
longest_word = ""
for word in words:
    if len(word) > len(longest_word):
        longest_word = word 
print (f"Longest word: {longest_word}")
    
#Define the vowels in the sentence, make use of if and else functions
vowels = ['a', 'e', 'i', 'o', 'u']
#Find out the number of vowels and consonants in each sentence 
vowel_counter = 0 
consonant_counter = 0
for char in sentence: 
#Exclude counting spaces by using the .isalpha function to let the computer search for only letters in the alphabet
    if char.isalpha():
#Let the computer understand that we are looking for both small and big letters
        if char.lower() in vowels:
#Add 1 to the vowel counter for each vowel found in the sentence otherwise add it to the consonant counter
            vowel_counter += 1
        else: 
            consonant_counter += 1
#Print vowels, consonants and words that are counted
print (f"Number of Vowels: {vowel_counter}")
print (f"Number of Consonants: {consonant_counter}")
print (f"Number of Words: {word_counter}")

