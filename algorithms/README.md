# ALGORITHMS

**Choose your favorite language (Rust would be advantages) to solve the following challenges:**

1. **FizzBuzz...But: You may heard the FizzBuzz task. Here we have the same rule. You will write a function fizzBuzz that receive a single parameter it will return the value base on these rule.**
	- If the input is divisible by 3, return 'Fizz'
	- If the input is divisible by 5, return 'Buzz'
	- If the input is divisible by both 3 and 5, return 'FizzBuzz'
    > BUT we're not allow you to use if/else statement. If there is any if or else word in your code. I will consider this question with 0 scores :(  
        
**Example**
```
fizzBuzz(21)
Fizz

fizzBuzz(25)
Buzz

fizzBuzz(45)
FizzBuzz
```

2.  **Bob has a server farm crunching numbers. He has nodes servers in his farm. His company has a lot of work to do. The work comes as a number workload which indicates how many jobs there are. Bob wants his servers to get an equal number of jobs each. If that is impossible, he wants the first servers to receive more jobs. He also wants the jobs sorted, so that the first server receives the first jobs. The way this works, Bob wants an array indicating which jobs are going to which servers.
Can you help him distribute all this work as evenly as possible onto his servers?**

**Example**

Bob has 2 servers and 4 jobs. The first server should receive job 0 and 1 while the second should receive 2 and 3.
```
distribute(2, 4) # => [[0, 1], [2, 3]]
 ```
On a different occasion Bob has 3 servers and 3 jobs. Each should get just one.
```
distribute(3, 3) # => [[0], [1], [2]]
```
A couple of days go by and Bob sees a spike in jobs. Now there are 10, but he hasn't got more than 4 servers available. He boots all of them. This time the first and second should get a job more than the third and fourth.
```
distribute(4, 10) # => [[0, 1, 2], [3, 4, 5], [6, 7], [8, 9]]
```

3. It's tricky keeping track of who is owed what when spending money in a group. Write a function to balance the books.
	- The function should take one parameter: a dict with two or more name-value pairs which represent the members of the  group and the amount spent by each.
    - The function should return a dict with the same names, showing how much money the members should pay or receive.
Further points:
	
    - The values should be positive numbers if the person should receive money from the group, negative numbers if they owe  money to the group.
    - If value is a decimal, round to two decimal places.

**Example:**
- 3 friends go out together: A spends $20, B spends $15, and C spends $10. The function should return an object/dict showing that A should receive $5, B should receive $0, and 
C should pay $5.
```
var group = {
    A: 20, 
    B: 15, 
    C: 10
}
 
splitTheBill(group) // returns {A: 5, B: 0, C: -5}
```
4.  **Fibonacci**
- The Fibonacci numbers are the numbers in the following integer sequence.
```
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, ……..
```
**In mathematical terms, the sequence Fn of Fibonacci numbers is defined by the recurrence relation**
- Fn = Fn-1 + Fn-2
- with seed values 
- F0 = 0 and F1 = 1.
- Given a number n, print n-th Fibonacci Number. 

1. **Palindrome**
   
**Given a string, write a function to check if it is palindrome or not.**
- In case: even you can reverse the string 
- In case: odd you should use the middle to split the word and then reverse the string  
**A string is said to be palindrome if the reverse of the string is the same as the string. For example, “abba” is Palindrome, but “abbc” is not Palindrome.**
```
Anna, civic, kayak, level, madam, mom, noon, racecar, radar, redder, refer, repaper, rotator, 12321, 15651
```

