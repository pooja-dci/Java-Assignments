## Book ArrayList Assignment
### Create a Book class with the following attributes:
- title
- author
- isbn (long)
- price
- isBorrowed
- [ ] one constructor that sets all attributes.
- [ ] follow the same drill : attributes will be `private` with `public` getters setters
- [ ] toString method to print all attribute values

### Demo.java class : **Outline of Demo.java attached in this respository**
- [ ] This class will have a static attribute which is an ArrayList of Book objects
- [ ] Inside the main method:
- [ ] Prompt the user to enter books details. 
- [ ] This data is used to create Book objects which are added to an ArrayList of books.
```
HINT: books.add(new Book(title, author, isbn, price, isBorrowed));
```
The program runs forever until the user types "done". When the user types "done" the list of books is displayed on the console.

Example Output:
```
Enter Book title (or 'done' to exit):
The Anatomy of Programming Languages
Author's name:
Alice E. Fischer
Book's isbn:
97801
Book's rental price
2.99
Is the book borrowed? (true/false)
false
Enter Book title (or 'done' to exit):
The Little Prince
Author's name:
Antoine de Saint
Book's isbn:
11634
Book's rental price
1.49
Is the book borrowed? (true/false)
true
Enter Book title (or 'done' to exit):
The Bench
Author's name:
Meghan The Duchess of Sussex
Book's isbn:
59343
Book's rental price
4.99
Is the book borrowed? (true/false)
true
Enter Book title (or 'done' to exit):
done
----
The books you entered are:

Book [title=The Anatomy of Programming Languages, author=Alice E. Fischer, isbn=97801, price=2.99, isBorrowed=false]

Book [title=The Little Prince, author=Antoine de Saint, isbn=11634, price=1.49, isBorrowed=true]

Book [title=The Bench, author=Meghan The Duchess of Sussex, isbn=59343, price=4.99, isBorrowed=true]

```
