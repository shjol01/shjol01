- 👋 Hi, I’m @shjol01
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
shjol01/shjol01 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
from statistics import mean
import statistics 
import timeit
import time  


start = time.time() 


NumList = []

   
Number = int(input("Please enter the Total Number of List Elements: "))



for i in range(1, Number + 1):
    value = int(input("Please enter the Value of %d Element : " %i))
    NumList.append(value)

n = int(input("Enter number of times to run the code: "))
for i in range(n):
    print("Run #",(i+1))

    NumList.sort()


    #list of numbers are : 6, 13, 21, 30, 40, 51, 63, 76
    
    # 8 Elements 
    print("The Smallest Element in this List is : ", NumList[0])
    
    
    print("The Largest Element in this List is : ", NumList[Number - 1])
    
    
    print("The Average Element in this List is  ",sum(NumList)/len(NumList))
    
    
    print("Median of the list of the number is : % s " % (statistics.median(NumList)))
    
    start, end = 0, 0
      
    
    if start < end: 
        
        NumList.extend(range(start, end)) 
     
        NumList.append(NumList) 
      
    print("range of the numbers are : ", (NumList)) 
    
    
    def tri_recursion(S):
      if(S > 5):
        result = S + tri_recursion(S - 1)
        print(result)
      else:
        result = 0
      return result
    
    print("\n\n List of the Numbers are : ")
    tri_recursion(13)
        
    end = time.time() 
    
    
    stop = timeit.default_timer() 
    print('Running time is: ', stop - start) 
    
    
        
