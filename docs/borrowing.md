# Borrowing
En Rust, el Borrowing es una característica que permite prestar una referencia a una variable en 
lugar de tomar la propiedad de ella. Esto significa que puedes utilizar la variable sin tener que 
transferir la propiedad de la misma, lo que te permite usarla tanto dentro como fuera de la función 
donde la prestaste.

### Ejemplo en Rust:
```rust
fn main() {
    let mut hola = String::from("Hola");
    cambiar(&mut hola);
    println!("{}", hola);
}

fn cambiar(algun_string : &mut String) {
    algun_string.push_str(", mundo!");
}
```
En este ejemplo, estamos prestando una referencia mutable a la variable `hola` al llamar a la función `cambiar()`

Más información en [**Rust Book: Referencias y Borrowing**](https://book.rustlang-es.org/rust-book-es/ch04-02-references-and-borrowing.html)