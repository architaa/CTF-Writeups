##Crypto Challenge - 2
The question was  



```
Breaking Bad Key Exchange
Hint 1 : in the range (1 to g*q), there are couple of pairs yielding common secrete as 399.
Hint 2 : 'a' and 'b' both are less than 1000.
```

Also there was an image given with the challenge which gave me the algorithm to write my code straigtaway  


![](/HACKIM-8/images/crypto2/1.png?raw=true)  

This was pretty simple. Just write a quick python code.  

```python
#!/usr/bin/env python

a=[]
b=[]



for x in range (1000):
	if (10**x % 541 == 298):
		a.append(x)

for y in range(1000):
	if (10**y % 541 == 330):
		b.append(y)

for value in a,b:
	print value
```  
```Output :  
      [170, 710]
      [268, 808]```
The flag was the commbination of the value in a and b. You might have to check for 4 combinations. And the below worked. 
###Flag:  


    flag{170, 808}
    
###Credits  
- Sagar Popat
- Archita Aparachita
- Pratap Chandra
- Chandrakant Nial
- Swaroop Yermalkar



