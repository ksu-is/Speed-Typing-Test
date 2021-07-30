import time
import math

ans='Y'
print(" "*7+"Welcome to Speed Test Program")
print("*"*44)
while(ans=='Y'):

# Starting the timer
    start_time = time.time()
    
    nouns = ("puppy", "car", "rabbit", "girl", "monkey")
    verbs = ("runs", "hits", "jumps", "drives", "barfs") 
    adv = ("crazily", "dutifully", "foolishly", "merrily", "occasionally")
    adj = ("adorable", "clueless", "dirty", "odd", "stupid")
    num = random.randrange(0,5)
    print (nouns[num] + ' ' + verbs[num] + ' ' + adv[num] + ' ' + adj[num])
    
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
if(ans=='N'):

    # Ending The Timer
    print("Thank You For Participating in My Program! Have a Nice Day")
