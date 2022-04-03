### Installing Rust

installing from the docs
Vs code extension: Rust (Its helps catch syntax errors and gives code snippets)

### Build Rust Code

main.rs

fn hello(){
println("helo world");
}

cmd: rustc .\main.rs
.\main.exe

### Build Rust Code with Cargo

Cargo(Package Management System) is same as npm in js.

cmd: cargo new newProject

Cargo.toml - is a package management file. Same as package.json in js.

cmd: cargo build
cmd: cargo run

### Variables and consoling

let a = 10;
let b = 20;
println("hello world, {} {}", a, b);

These curly varibales represents variables

### Variables types(scaler)

1. integers - unsigned(a number cannot be negative)
   signed(can be negative)

let unsigned: u8 = 10;
// u8, u16, u32, u64, u128

1 1 1 0 1 1
2to5 2to4 2to3 2to2 2to1 2to0

let signed: i8 = -10;

2. floats: f32 = 1.0;

3. char

let letter = "c";
let emoji = "\u{1F600}"; //:D

4. boolean

let is_true: bool = true;

### Arrays (compound)

let arr: [u8; 3] = [1,2,3];
let other_arr: [u8; 5] = [100; 5];

println!("index: {}, length: {}", arr[0], other_arr.len());

//print strcture of array and other objects
println!("{:?}", other_arr)

### Varibales (tuple)

tuple can hold multiple elements of different types together

fn main(){
let tuple: (u8, bool, f32) = (5, true, 2.1);
let tuple2 = (3, 5);

     //print the structure

    println!("first {}, second {}, third {}, tuple.0, tuple.1, tuple.2);
    println!("{:?}", tuple2);

    let (a, b, c) = tuple;

    //destructing
    println!("first {}, second {}, third {}", a, b, c);

}


### functions

fn main() {
    println!("{}", id_even(2));
}

//all rust is default private

pub fn is_even(num: u8) -> bool{
    let digit: u8 = num % 2;
    digit == 0 // return not needed ;
}

### mutability

mut means can be change;

fn main(){
    let mut num = 5;
    num = 3;
    println!("{}", num);
}

### Arrays and slices

fn main() {
    let arr = [0,1,2,3]; //length
    let slice = &arr[1 .. 3]; // [1,2] subarray // dont know the length during compile time
}

fn borrowing_slice(arr: [u8, 4], slice: &[u8]){
    println!("{:?}, arr);
    println!("{:?}, slice);
    println!("length: {}", slice.len());
    println!("{} {}", slice[0], slice[1]);
}


### Strings

fn main(){
    let str: &str = "hello world"; 
    let mut string: String = String::from("hello world"); // string object, dynamic size array

    let slice = &string[.. 6]; // get everything from index 0 to till 6
    slice.len();

    string.push('1');
    string.push_str("! Bob);
    string = string.replace("hello", "bye");

    println!("{}", string);

}

### if statements

let n = 3;
if n > 0 {
    println!("{}", n);
} else if n < 0{

}

### for loop

for i in 0..6 {
    println!("{}", i);
}


### while loop

let mut i = 0;
while i < 4 {
    println("{}", i);
    i += 1;
    if i == 3 {
        println!("exit");
        break
    }
}

### match (Switch)

let i = 5;
match i {
    0 => println!("0");
    1 | 2 => println("1,2");
    3..=4 => println("3,4");
    _ => println("default");
}


### structs

fn main() {
    let name = String::from("Bird")
    let bird = Bird { name, attack: 5 };
    bird.print_name();
}

struct Bird {
    name: String, 
    attack: u64
}

impl Bird {
    fn print_name(&self){
        println("{}", self.name)
    }
}

### traits

