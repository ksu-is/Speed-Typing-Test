import time
import math

ans='Y'
print(" "*7+"Welcome to Speed Test Program")
print("*"*44)
while(ans=='Y'):

# Starting the timer
    start_time = time.time()
text=input("\nEnter text: ")

# Ending the timer
end_time=time.time()

# Counting total number of words typed by the used in that time frame
text=text.split(" ")
word_count=0
for i in text:
    word_count +=1
