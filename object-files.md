## Writing and Reading objects to a file

Use the Car.java class you created in the previous assignment

>Serialization is the conversion of an object to a series of bytes , so that the object can be easily saved to persistent storage or streamed across different platforms or network. The same byte stream can then be deserialized - converted into a replica of the original object. As byte stream is platform neutral, objects created in one system can be deserialized in other platform. It is very useful when you want to transmit one object data across the network, or from one JVM to another. 
A Java object is serializable if its class or any of its superclasses implements the `java.io.Serializable` interface
### Step 1: 
Make the Car class `implement Serializable` interface

### Step 2: 
In your Demo.java, inside the main method - create 2 Car objects. I am calling my objects `honda , fiat`. You can give the objects any name you wish.
Conceal the checked IOException by declaring main method with `throws IOException, ClassNotFoundException` decleration. You will change this to a try catch block in Step 5
>The objects can be converted into byte-stream using `java.io.ObjectOutputStream`. In order to enable writing of objects into a file using `ObjectOutputStream`, it is mandatory that the concerned class implements Serializable interface as mentioned in step 1. Reading objects in Java are similar to writing object and it uses `ObjectInputStream`. On reading objects, the ObjectInputStream directly tries to map all the attributes into the class into which we try to cast the read object. If it is unable to map the respective object exactly then it throws a ClassNotFound exception.

### Step 3:
Now, continue coding inside the main method. Let's write the 2 objects into a file called cars.txt which would reside inside our current working directory
```
FileOutputStream fileStream = new FileOutputStream(new File("./cars.txt")); //Relative Path
ObjectOutputStream objectStream = new ObjectOutputStream(fileStream);
		
objectStream.writeObject(honda);
objectStream.writeObject(fiat);

objectStream.close();
fileStream.close();
```

### Step 4:
Let's read the object file back into 2 Car objects














