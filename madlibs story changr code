with open("story.txt","r") as f:
    story=f.read()

start=-1
target_start="<"
target_end=">"
words=set()

for i,char in enumerate(story):
    if char==target_start:
        start=i

    if char==target_end and start!=-1:
        words.add(story[start:i+1])

answers={}
for k in words:
    ch=input("Enter your preffered word for "+k+": ")
    answers[k]=ch

for k in words:
    story=story.replace(k,answers[k])

print("\n",story)
