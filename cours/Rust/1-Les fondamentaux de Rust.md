#rust #cours

## Variables et Mutabilité

Par défaut, les variables en Rust sont immuables. Cela signifie que leur valeur ne peut pas changer une fois qu'elles sont attribuées. Pour rendre une variable mutable, Il faut utiliser le mot-clé `mut`.


```rust
fn main() 
{     
	let immuable = 5;
	let mut mutable = 5;
	println!("La valeur immuable est: {}", immuable);
	mutable += 1; 
	// ceci est permis car 'mutable' est déclarée mutable     
	println!("La valeur mutable est: {}", mutable); 
}
```

## Types de Données

Rust est un langage typé statiquement, ce qui signifie que le type de chaque variable doit être connu au moment de la compilation. Quelques types de données de base :

### Entiers


```rust
fn main() 
{     
	let x: i32 = -123; // 32-bit signed integer     
	let y: u32 = 123; // 32-bit unsigned integer     
	println!("x = {}, y = {}", x, y);
}
```

### Flottants

```rust
fn main() 
{     
	let x = 2.0; // f64, double precision float     
	let y: f32 = 3.0; // f32, single precision float     
	println!("x = {}, y = {}", x, y); 
}
```

### Booléens

```rust
fn main() 
{     
	let t = true;     
	let f: bool = false; // with explicit type annotation     
	println!("t = {}, f = {}", t, f); 
}
```

### Caractères


```rust
fn main() 
{     
	let c = 'z';     
	let z: char = 'ℤ'; // with explicit type annotation     
	let heart_eyed_cat = '😻';     
	println!("c = {}, z = {}, cat = {}", c, z, heart_eyed_cat); 
}
```

## Fonctions

Les fonctions sont déclarées avec le mot-clé `fn`. Elles peuvent prendre des paramètres et retourner une valeur.


```rust
fn main()
{     
	let result = add(1, 2);     
	println!("1 + 2 = {}", result); 
}  

fn add(x: i32, y: i32) -> i32 
{     
	x + y // pas besoin de `return` ici; Rust retourne la dernière expression 
}
```

## Contrôle de Flux

Rust fournit plusieurs structures de contrôle, y compris `if`, `else`, et `loop`.

### Conditionnelle if


```rust
fn main() 
{     
	let number = 6;      
	if number % 4 == 0 { println!("Le nombre est divisible par 4"); } 
	else if number % 3 == 0 { println!("Le nombre est divisible par 3"); } 
	else if number % 2 == 0 { println!("Le nombre est divisible par 2"); } 
	else { println!("Le nombre n'est divisible ni par 4, ni par 3, ni par 2"); } 
}
```

### Boucles

Rust propose plusieurs types de boucles: `loop`, `while`, et `for`.

```rust
fn main() 
{     
	// loop infini     
	loop 
	{    
		println!("Encore !");         
		break; // Arrête la boucle     
	}     
	 
	// while     
	let mut number = 3;     
	while number != 0 
	{         
		println!("{}!", number);         
		number -= 1;     
	}     
	println!("DÉCOLLAGE !!!");  
	    
	// for avec une gamme     
	for number in 1..4 { println!("{}", number); }
}
```

[[1.1-Fonction avancée - Ownership]]
[[1.2-Fonction avancée - Slice]]
[[1.3-Fonction avancée - Enums & Pattern Matching]]
[[1.4-Fonction avancée - Erreurs & Concurrency]]
[[1.5-Fonction avancée - Traits & Pointers]]
[[1.6-Fonction avancée - Lifetimes & Macro]]
[[1.7-Fonction avancée - Pattern Matching]]



