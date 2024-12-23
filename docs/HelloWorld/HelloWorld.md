# Hello World in Tea
First, we're going to want to write our main function.  
This will be the entry point of our program.
```tea
uint16_t main()
    return 0;
end
```

Here, we are:  
Declaring the function (`uint16_t main`) that will return a `uint16_t` (unsigned 16 bit integer) that takes no arguments (`()`),  
exiting with a return value of zero (`return 0;`),  
ending the function definition (`end`).

Next, we should probably add some IO.  
Let's print something to the screen.  
But what to print?

We will print `Hello Tea!`.  
We can make a string holding the value `Hello Tea!` by adding this line to our code.  
```tea
    const char[?] hello = "Hello Tea!";
```

This code creates a constant (`const`) array of char (`char[]`) with a size decided at compile time (`[?]`).  
This means the array's size is decided by the compiler based off of what we initially set it to; and it will not be changed.  

We can use this array in a function call like so.
```tea
    puts(hello,newline=true);
```

This code passes our string into the built-in function `puts()`.  
This built-in function by default doesn't put a new line character after our string, so we must specify that by ourselves using the keyword argument `newline` (`newline=true`).

Our final code:
```tea
uint16_t main()
    const char[?] hello = "Hello Tea!";
    puts(hello,newline=true);
    return 0;
end
```

[Return to home page](../Tea.md)