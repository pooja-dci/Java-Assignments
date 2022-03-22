## Lab - 1
- Non graded and closed book - you can use class resources and textbook. 
### Programming Fundamentals:
#### Most of the programs from questions 1-8 can be written inside the main method or other static methods without having to use OOP concepts.
#### Create one project and have your solutions for each question in the same project. Class names can be the question numbers like Solution1, Solution2..and such

1. Write a program to reverse the order of words in a sentence
> This question involves String concepts. .split(" ") method i.e split by space, might be helpful here
- Use your palindrome assignment for reference if needed

Sample Output: 
```
Enter a sentence and the words will be printed in reverse order:
The first program everyone writes is Hello World
Sentence reversed: World Hello is writes everyone program first The 
```

2. Write a program to ask the user to enter a year and tell them if it's a leap year or not
- A leap year is divisible by 4 but not divisible by 100, OR it is divisible by 400
- HINT: % operator can be used to check if a number is divisible by another number. If the number is divisible % will be equal to 0
>This question involves logical operators and conditional statements

Sample output 1:
```
Enter a year: 
1991
The year you entered is not a leap year
```
Sample output 2:
```
Enter a year: 
2012
The year you entered is a leap year
```

3. Write a program that declares and initializes a counter to 0. Run a forever **while loop**, increment counter by 1 with every iteration. break the loop when counter is 5. continue the loop without printing the number when counter is 3. Print the counter for all other values.
>This question involves while loop, break and continue statements

Expected output:
```
1
2
4
```

4. Write a program to initialize an array of 5 float numbers. Loop through the array using a **for loop** and print each number.
>This question involves array (which can hold primitive and is of fixed size) and for loops 

Sample output:

```
2.5
4.8
9.07
12.55
55.7
```

5. Write a program to ask the user for a decimal number, and print the floor, ceil, round of that number
>This question involves java.lang.Math class

Sample Output 1:
```
Enter a decimal number:
2.85
The ceil value of the number is 3.0
The floor value of the number is 2.0
The number rounded to its nearest integer is 3
```

Sample Output 2:
```
Enter a decimal number:
1.25
The ceil value of the number is 2.0
The floor value of the number is 1.0
The number rounded to its nearest integer is 1
```

6. Write a program to ask the user for states they have visited in the US. Ignore case by converting their input to lower case. **Ignore** duplicate inputs. Order of input doesn't matter. The program runs forever until the user types "done". When the user types "done", display the unique list of states back to the user.
>Use one of the collection framework classes

Sample Output:
```
Enter the states you have visited one at a time.
State name: 
NEW JERSEY
State name: 
NEW YORK
State name: 
new YORK
State name: 
Arizona
State name: 
Washington
State name: 
WASHINGTON
State name: 
new jersey
State name: 
MaInE
State name: 
maine
State name: 
done
[maine, arizona, new jersey, washington, new york]
```

7. Write a program that asks user for 2 integers and print the divison of the 2 integers. Handle ArithmeticException and print its stacktrace. Handle all other RuntimeException and print its message. Irrespective of whether an exception ocurred or not, print a "Thank you" message. 

8. Write a program that counts the occurances of each word in a text file (the_prince_quotes.txt in the same repository). Make it case-insensitive by coverting each word to lower case before counting
>Involves text file reading, using String's .split() method, using HashMap to store the word to count mapping

Sample Output:
```
{explain=1, very=2, victories=1, butterflies=1, invisible=1, when=1, beautiful=1, children=2, far=1, else=1, usually=1, because=1, presence=1, if=1, they=2, you=3, in=1, rightly=1, is=12, them=2, it=4, am=2, something=1, eye=1, himself=1, ups=2, acquainted=1, must=1, looking=1, endure=1, become=2, touched=1, be=2, ahead=1, secret=2, our=2, eyes=1, thinking=1, seen=2, remember=1, see=2, world=1, are=3, mysterious=1, by=1, have=3, grown=2, place=1, man=1, so=1, can't=1, a=3, one=3, loves=1, i=5, people=1, the=15, straight=1, such=1, sunset=1, cannot=1, to=7, understood=1, thing=2, did=1, essential=1, but=4, sometimes=1, tedious=1, simple=1, him=1, wish=1, that=4, biggest=1, only=3, things=2, besides=1, few=2, all=1, need=1, felt=1, my=1, look=1, heart=3, most=1, important=1, never=2, once=1, defeats=1, were=1, know=1, who=1, here=1, blind=1, tears=1, rather=1, for=1, anything=2, can=1, not=2, perhaps=1, caterpillars=1, and=4, now=1, of=4, sad=1, themselves=1, land=1, conceited=2, hear=2, or=1, again=1, go=1, praise=1, with=4, what=2, well=1, time=1, he=1}
```

### OOP Concepts (HOMEWORK for the next 2 days):
#### This question would involve following basic OOP principles and coding principles like single-responsibility, DRY and YAGNI principles. Each entity will be created in it's own class. main method will be in a seperate class and that'll be the one interacting with the user.

9. Create a Song class with the following attributes

* title
* duration

Create a PlayList class which has instance attributes
* name
* ArrayList of Songs called playList
* Methods:
* Print all songs in the playlist
* Find song by name : findSong(String song) returns true if the song name is present in the playList
HINT: .getName().equals()

Create a Main class with the main method
* Create an object of PlayList, give it a name and an empty arraylist to begin with
* Create some Song objects and add it to object's playList
* Print all the songs in the playlist
* Find a song in the playlist

Write the playlist object to an object file.
