##BASICS-2

* **While Loop**    
```
while a_logical_op:
	type ops that 
	have done in
	each turn
	as intended
```
* In python, ':' should be followed by indentation.(for,while,if, elif, else...)  

* **Logical Ops**
```
==  : equals
!=  : not equal
>   : greater
<   : smaller
>=  :greater and equal
<=  :smaller and equal
and :logical and
or  :logical or
```
* **For Loop**
```
for y in range(start,end,amout of increasing):
	type ops that 
	have done in
	each turn
	as intended

```   
* **Break**
Stops loop. Using with if statements.   

* **Continue**
Stops current turn(skip ops below continue) and go to next turn   
* **To call a command from system** 
import os then `os.system("COMMAND")`     

* `pass` can be used as break   
* **Date Time**    
import datetime 
	* to get todays date `datetime.date.today()`
	* to get tomorrow 

	```
	today = datetime.date.today()
 	temp=datetime.timedelta(days=1)
 	today+temp #returns tomorrow
	```
	* to format date `today.strftime("%m/%d/%Y %A %B")`
	to get a spesific date `datetime.date(2015,12,25)`
   
    
    

**CODE**
```
#!usr/bin/python
import os
import datetime
import time
#___________________WHILE LOOP___________________
x=0
while x<=100 :
	print x
	x=x+5 


print "end of loop"

time.sleep(1)
#Print animated text
z="Welcome to My Universe!!!"
t=0
while t <= len(z):
	os.system("clear")
	print z[:t]
	time.sleep(.15)
	t=t+1


#___________________FOR LOOP______________________

for y in range(1,17,3):
	print "y is ", y




#___________________CALLING SYS COMMAND____________
print "print via python"
os.system("echo 'print via Bash'") #prints in cli via bash
#os.system("sudo apt-get update") #update repos


#_________________DATETIME____________
today = datetime.date.today()
print "today is", today

temp=datetime.timedelta(days=1) #returns 1 day
print "tomorrow is", today+temp #prints tomorrow

print today.strftime("Today is %m/%d/%Y %A %B")



fitr=datetime.date(2015,7,17)
print "Eid al Fitr is ",fitr
left=fitr-today
print left,"left to Eid al Fitr"


```