Create an ArrayList of your favorite tv show names. 
My tvshows ArrayList looks like below code. Yours can be different.

```
		ArrayList<String> tvshows = new ArrayList<String>();
		
		tvshows.add("The Office");
		tvshows.add("Seinfeld");
		tvshows.add("Friends");
		tvshows.add("Parks and Rec");
		tvshows.add("Silicon Valley");
		tvshows.add("Zindagi Gulzar Hai");
		tvshows.add("Saans");
		tvshows.add("Planet Earth");
    
```
4 ways to iterate over an ArrayList:

1. for loop
```
		for(int i = 0; i <= tvshows.size()-1 ; i++) {
			
			System.out.println(tvshows.get(i));
		}
```
2. for-each loop
```
		for(String show : tvshows) {
    
			System.out.println(show);
		}
```
3. Using ListIterator - you can use this method when you want to modify the ArrayList while looping through it
```
		ListIterator iterate = tvshows.listIterator();
		
		while(iterate.hasNext()) {
			
			System.out.println(iterate.next());
		}
```
4. Using lambda expression. This method was introduced in Java 8. So you can find it in newer versions of Java.
```
		tvshows.forEach(tvshow -> System.out.println(tvshow));
```

