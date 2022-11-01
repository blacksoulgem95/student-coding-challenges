# Roman to Integer

I numeri romani sono rappresentati da sette diversi simboli: I, V, X, L, C, D e M.

| **Simbolo** | **Valore** |
|-------------|------------|
| I           | 1          |
| V           | 5          |
| X           | 10         |
| L           | 50         |
| C           | 100        |
| D           | 500        |
| M           | 1000       |

Ad esempio, 2 è scritto come II in numero romano, sono solo due uno sommati. 
12 è scritto come XII, che è semplicemente X + II. 
Il numero 27 è scritto come XXVII, che è XX + V + II.

I numeri romani sono generalmente scritti dal più grande al più piccolo da sinistra a destra. 
Tuttavia, il numero per quattro non è IIII. Invece, il numero quattro è scritto come IV. 
Poiché l'uno è prima del cinque lo sottraiamo facendo quattro. 
Lo stesso principio si applica al numero nove, che è scritto come IX. 
Esistono sei casi in cui viene utilizzata la sottrazione:

 - I può essere posizionato prima di V (5) e X (10) per fare 4 e 9.
 - X può essere posizionato prima di L (50) e C (100) per fare 40 e 90.
 - C può essere posizionato prima di D (500) e M (1000) per fare 400 e 900.
 
Creare una funzione che, dato un numero romano denominato `s`, lo converta in un numero intero.
 
## Esempi

### Esempio 1
```
Input: s = "III"
Output: 3
Spiegazione: III = 3.
```

### Esempio 2
```
Input: s = "LVIII"
Output: 58
Spiegazione: L = 50, V= 5, III = 3; cioè 50 + 5 + 3 = 58.
```

### Esempio 3
```
Input: s = "MCMXCIV"
Output: 1994
Spiegazione: M = 1000, CM = 900, XC = 90 and IV = 4; cioè 1000 + 900 + 90 + 4.
```

## Condizioni
 - La stringa in input `s` è un numero romano tra 1 e 15 caratteri in lunghezza
 - La stringa in input `s` contiene solo i seguenti caratteri: `('I', 'V', 'X', 'L', 'C', 'D', 'M')`
 - È garantito che la stringa in input `s` sia un numero romano valido nell'intervallo $[1, 3999]$
