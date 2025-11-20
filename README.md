## Experiment 6 – Create an Application to Demonstrate Vector Collection Object  

<H3>ENTER YOUR NAME: J.F.SHARON ARUL BHARATHI </H3>  
<H3>ENTER YOUR REGISTER NO: 212224100056</H3>  
<H3>EX.NO.6</H3>  
<H3>DATE: 20/11/2025</H3>  

<H1 ALIGN =CENTER> Demonstrating Vector Collection in Rust </H1>  

## AIM:  
To create a Rust application that demonstrates the use of the Vector (Vec) collection object.  

## EQUIPMENTS REQUIRED:  
- Hardware – PCs  
- Software – Visual Studio Code (Version 1.104.0)  
- Rust Installation  

## RELATED THEORETICAL CONCEPT:  

*Vectors in Rust:*  
A Vector (`Vec<T>`) is a growable array type in Rust. Unlike arrays, vectors can change their size at runtime by adding or removing elements.  

*Key Features of Vectors:*  
- Store a collection of values of the same type.  
- Grow dynamically as elements are inserted.  
- Provide indexing and safe element access using `.get()`.  
- Can be traversed using loops and iterators.  

## ALGORITHM:  
STEP 1: Start the program. <BR>  
STEP 2: Import the standard library (no external crates required). <BR>  
STEP 3: Define the `main` function. <BR>  
STEP 4: Create a new Vector using `Vec::new()` or the `vec![]` macro. <BR>  
STEP 5: Insert values into the vector using `.push(value)`. <BR>  
STEP 6: Iterate and print the elements of the vector. <BR>  
STEP 7: Access elements using indexing and `.get(index)`. <BR>  
STEP 8: End the program. <BR>  

## PROGRAM:  
```

fn main() {
    let mut numbers: Vec<i32> = Vec::new();

    numbers.push(10);
    numbers.push(20);
    numbers.push(30);
    numbers.push(40);
    numbers.push(50);

    println!("Elements of the vector:");
    for num in &numbers {
        println!("{}", num);
    }


    println!("\nAccessing elements:");
    println!("First element (using index): {}", numbers[0]);
    
    match numbers.get(2) {
        Some(value) => println!("Third element (using get): {}", value),
        None => println!("No element found at index 2"),
    }

    numbers.pop();
    println!("\nAfter removing the last element:");
    for num in &numbers {
        println!("{}", num);
    }
}


```
## OUTPUT:

<img width="915" height="513" alt="image" src="https://github.com/user-attachments/assets/2570d362-562e-43fe-9175-2b56e7674e50" />


## RESULT:

Thus we have successfully created a Rust application that demonstrates the use of the Vector (Vec) collection object.
