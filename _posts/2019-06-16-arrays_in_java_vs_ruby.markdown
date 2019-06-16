---
layout: post
title:      "Arrays in Java Vs Ruby"
date:       2019-06-16 22:30:08 +0000
permalink:  arrays_in_java_vs_ruby
---


Think all programming languages are created equal? Not really. Back in college when I took programming classes I always thought language creators were trying way to hard just to make learning programming very difficult. Popular language like JAVA were very hard to understand because it was so different than human language like “English”. For past month, I have been learning Ruby and I have found it to be much more “human – friendly” language.

Lets see an example of simple Array: 
In JAVA, if we like to declare an array of “cars” then we would write :

```
String[] cars; 
String[] cars = {"Volvo","BMW","Ford","Mazda"};
```



Not so bad so far, but lets iterate through array and print out the element of the array:
```
    for(int i =0; i <cars.length; i++) {
     System.out.println(cars[i]);
    } 
```
Output:
```
Volvo
BMW
Ford
Mazda
```

In Ruby, we can achieve the same result by simply doing the following:
```
	cars = ["Volvo","BMW","Ford","Mazda"]
	cars.each do |car|
		puts car
	end
```


Better, but still not that different from JAVA. But, what if we have an array of arrays. In JAVA, it is known as multi-dimensional array. Lets look at this example of iterating through multi-dimensional array.

```
 int[][] myNumbers = { {1, 2, 3, 4}, {5, 6, 7} };
   for (int i = 0; i < myNumbers.length; ++i) {
    for(int j = 0; j < myNumbers[i].length; ++j) {
   System.out.println(myNumbers[i][j]);
    }
   }
```
Output:
```
1
2
3
4
5
6
7
```
Lets look at Ruby code for doing the same thing.

```
  myNumbers = [[1,2,3,4],[5,6,7]]

  myNumbers.each do |number_array|
    number_array.each do |number|
    puts number
    end
  end
```

  This one definitely look much more readable. Its just few examples that I am comparing here but simplicity of Ruby is amazing. It may be the start of my journey of learning to code but I am loving Ruby so much. I am thankful to its developer Yukihiro Matsumoto, its because of him, learning to code is fun again!!

