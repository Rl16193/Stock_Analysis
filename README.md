# Stock_Analysis

Use VBA to write a code Which will help in performing automated analysis on the stock options

## Overview

Steve's parent has asked him to invest their money in stock. They wanted to invest in DAQO stocks but initial analysis showed that these stocks might not be a good investment. 
>At the click of a button, he can analyze an entire dataset. Now, to do a little more research for his parents, he wants to expand the dataset to include the entire stock market over the last few years

Initial code had a longer run time. We are looking to refactor the code and improve it performance.

## Results

![2017](https://user-images.githubusercontent.com/100053788/158299557-8acc4041-70e3-4a6e-9875-bb8ac71ae710.PNG)

**Report for Year 2017**

![2018](https://user-images.githubusercontent.com/100053788/158299559-e99a7513-0109-4a67-a2e2-4b8ebe534c45.PNG)

**Report for Year 2018**

### Analysis of Stock Returns

1. First look shows that almost all the stocks fared poorly over the course of the analysis. The % returns have reduced.
2. The only stocks giving positive return over the analysis period are RUN and ENPH. 
3. The TERP stock shows improvement from **-7.2%** to **-5.0%**
4. DQ stocks performed well in the year 2017 but was unable to provide a positive return in 2018.
5. The worst return is observed is stock SEDG reduvcing from **184.5% to -7.8%**

![VBA_Challenge_2017](https://user-images.githubusercontent.com/100053788/158301323-79539496-691d-4b48-afc8-32c392432a27.PNG)

**Runtime - 2017**

![VBA_Challenge_2018](https://user-images.githubusercontent.com/100053788/158301327-66c69f9b-24e3-4527-ba67-a831a676d4db.PNG)

**Runtime - 2018**

### Analysis of Runtime

The initial runtime of the code was a bit longer as we have to run a nested loop which creates 12 * 3013 iterations.
The refactored code utilizes a single loop and uses array to store the data of the stocks, which saves the runtime of the code. **Reduces runtime from .48 secs to 0.07 sec**

## Summary

### Advantage of refactoring the VBA Script

Refactored Code has a shorter run time making the code much more efficient.

### Disadvantage of refactoring the VBA Script

Rewriting a code using a different flow of logic takes some time to understand and can create errors.

### Pros of Refactoring

[https://stackoverflow.com/questions/43983284/what-are-the-advantages-and-disadvantages-of-refactoring-code-smell-in-software#:~:text=Nonetheless%2C%20the%20most%20obvious%20advantage,pipeline%20and%20your%20automated%20tests.](StackOverflow - Advantage and Disadvantage of Refactoring code)
1. Refactoring Improves the Design of Software
2. Refactoring Makes Software Easier to Understand
3. Refactoring Helps Finding Bugs
4. Refactoring Helps Programming Faster

### Cons of Refactoring

[https://stackoverflow.com/questions/43983284/what-are-the-advantages-and-disadvantages-of-refactoring-code-smell-in-software#:~:text=Nonetheless%2C%20the%20most%20obvious%20advantage,pipeline%20and%20your%20automated%20tests.](StackOverflow - Advantage and Disadvantage of Refactoring code)
 1. It's risky when the application is big 
 2. It's risky when the existing code doesn't have proper test cases 
 3. It's risky when developers do not understand what's all about
