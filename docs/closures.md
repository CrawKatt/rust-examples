# Closures
Los Closures son funciones anónimas que se pueden almacenar en variables o pasar como argumentos a otras funciones
### Ejemplo en Rust:
```rust
fn main() {
    let suma = |a: i32, b: i32| -> i32 {
        a + b
    };
    
    let resultado = suma(5,5);
    println!("{}", resultado);
}
```

Más información en [**Rust Book: Closures**](https://book.rustlang-es.org/rust-book-es/ch13-01-closures.html)