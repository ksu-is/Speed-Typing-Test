import time
import math
import random

ans='y'
print(" "*7+"Welcome to Speed Test Program")
print("*"*44)
while(ans=='y'):
    # Starting The Timer
    start_time = time.time()
    print("Enter the phrase: ")
    phrase1 = ("puppy", "car", "rabbit", "girl", "monkey", "My", "")
    phrase2 = ("runs", "hits", "jumps", "drives", "barfs", "wife") 
    phrase3 = ("crazily", "dutifully", "foolishly", "merrily", "occasionally","cooks")
    phrase4 = ("adorable", "clueless", "dirty", "odd", "stupid", "amazingly")
    num = random.randrange(0,5)
    print (phrase1[num] + ' ' + phrase2[num] + ' ' + phrase3[num] + ' ' + phrase4[num])
    
    text=input("\nEnter The Text: ")
    
    # Ending the timer
    end_time=time.time()
    # Counting total number of words typed by the used in that time frame
    text=text.split(" ")
    word_count=0
    for i in text:
        word_count +=1
    # Printing the typing speed of the user
    print("Your typing speed is : {0:.2f}".format(word_count*60/(end_time - start_time))+" WPM (Words Per Minute)")
    ans=input("Do you want to continue ? (Y/N): ")
if(ans=='n'):
    # Ending The Timer
    print("Thank You For Participating in My Program! Have a Nice Day")
