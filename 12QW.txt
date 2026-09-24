fn main() {
    // 1. Hello World
    println!("Hello, world!");

    // 2. 变量与基本运算
    let a = 10;
    let b = 20;
    let sum = a + b;
    let product = a * b;
    println!("a = {}, b = {}", a, b);
    println!("sum = {}, product = {}", sum, product);

    // 3. 调用自定义函数
    let result = add(3, 5);
    println!("add(3, 5) = {}", result);

    // 4. for 循环
    println!("Counting from 1 to 5:");
    for i in 1..=5 {
        println!("  {}", i);
    }

    // 5. 使用 Vec 遍历
    let fruits = vec!["apple", "banana", "cherry"];
    for fruit in &fruits {
        println!("I like {}", fruit);
    }

    // 6. match 表达式
    let number = 7;
    match number {
        1..=5 => println!("{} is small", number),
        6..=10 => println!("{} is medium", number),
        _ => println!("{} is large", number),
    }
}

// 一个简单的加法函数
fn add(x: i32, y: i32) -> i32 {
    x + y
}
