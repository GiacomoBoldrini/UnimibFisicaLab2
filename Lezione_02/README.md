# Lezione 2: ripasso di ```C``` ed introduzione al ```C++```, parte 2

## 2.1 Variabili e puntatori

![linea](immagini/linea.png)

### 2.1.1 La gestione delle variabili nel calcolatore

  * In un computer tutto è rappresentato mediante **numeri**
  * I numeri sono salvati in **zone di memoria** (Random Access Memory = RAM)
  * Le celle della memoria sono individuate mediante **indirizzi**
  * Le **variabili di diversi tipi occupano una o piu' celle** di memoria (una zona),
    a seconda del tipo
    * Il calcolatore e' in grado di **interpretare correttamente il contenuto** di una zona di memoria, 
      se conosce l'indirizzo della prima cella ed il tipo salvato

![cella](immagini/celle.png)

![linea](immagini/linea.png)

### 2.1.2 Lo spazio occupato dalle variabili 

  * ogni tipo ha una **dimensione assegnata** nella RAM
  * per i tipi numerici interi, una dimensione assegnata significa che **i valori che la variabile puo' assumere
    sono limitati**
  * i tipi in virgola mobile (```float```, ```double```) non hanno limitazioni in valore, ma in precisione,
    quindi il tipo ```double```, occupando piu' celle di memoria, e' piu' preciso del tipo ```float``` 
  * per conoscere la dimensione occupata da un tipo, si puo' utilizzare la funzone ```sizeof ()```:
    ```cpp
    std::cout << "Dimensione di un char : " << sizeof (char)  
             << " byte" << std::endl ; 

    ```

![linea](immagini/linea.png)

### 2.1.3 Le dimensioni tipiche di alcuni tipi 

  * a seconda dell'architettura del calcolatore che si sta utilizzando, 
    le **dimensioni di un tipo possono cambiare**
  * nella tabella che segue,
    sono indicati **valori tipici** per le dimensioni dei tipi comunemente utilizzati
  * esistono **type modifier** che cambiano le caratteristiche di un tipo 
    (```signed```, ```unsigned```, ```short```, ```long```)
    che ne modificano la dimensione o l'intervallo di copertura

 | tipo | dimensione (in Byte) | intervallo |
 | --- | :---: | :---: |
 | short int              | 2      | -32,768 to 32,767               |   
 | unsigned short int     | 2      | 0 to 65,535                     |               
 | unsigned int           | 4      | 0 to 4,294,967,295              |                      
 | int                    | 4      | -2,147,483,648 to 2,147,483,647 |                 
 | long int               | 4      | -2,147,483,648 to 2,147,483,647 |                 
 | unsigned long int      | 4      | 0 to 4,294,967,295              |    
 | long long int          | 8      | -(2^63) to (2^63)-1             |     
 | unsigned long long int | 8      | 0 to 18,446,744,073,709,551,615 |                 
 | signed char            | 1      | -128 to 127                     |               
 | unsigned char          | 1      | 0 to 255                        |            
 | float                  | 4      |                                 |                      
 | double                 | 8      |                                 |                      
 | long double            | 12     |                                 |                        
 | wchar_t                | 2 or 4 | 1 wide character                |                    


![linea](../immagini/linea.png)

### 2.1.4 L'indirizzo di memoria: i puntatori

  * l'indirizzo di una cella di memoria e' un numero, 
    quindi puo' essere a sua volta **salvato in una variabile**
  * variabili che contengono indirizzi alla prima cella di memoria di altre variabili 
    sono chiamate **puntatori**
  * siccome rivestono un ruolo fondamentale nella programmazione,
    si **dichiarano in modo specifico**, con la sintassi ```type * var```:
    ```cpp
    int * puntatore_ad_intero ;

    ```
  * questa dichiarazione fa si' che **il programma sappia come accedere al contenuto**
    della cella di memoria che sta all'indirizzo salvato in ```puntatore_ad_intero```,
    perche' sa di che tipo si tratta

![cella](immagini/puntatore.png)

![linea](immagini/linea.png)

### 2.1.5 Dalla variabile al puntatore e viceversa

![linea](immagini/linea.png)

### 2.1.6 Esempi sull'uso dei puntatori

![linea](immagini/linea.png)

### 2.1.7 Puntatori ed array

![linea](immagini/linea.png)

### 2.1.8 I puntatori sono variabili

![linea](immagini/linea.png)

### 2.1.9 Le referenze

![linea](immagini/linea.png)

### 2.1.10 Riepilogo sui puntatori

![linea](immagini/linea.png)

## 2.2 Il passaggio di parametri alle funzioni

![linea](immagini/linea.png)

### 2.2.1 Passaggio per valore

![linea](immagini/linea.png)

### 2.2.2 Passaggio per puntatore

![linea](immagini/linea.png)

### 2.2.3 Passaggio per referenza

![linea](immagini/linea.png)

## 2.3 La gestione dinamica della memoria

![linea](immagini/linea.png)

## 2.3.1 Heap and Stack

![linea](immagini/linea.png)

## 2.3.2 Allocazione di una variabile nella Stack

![linea](immagini/linea.png)

## 2.3.3 Allocazione di una variabile nella Heap

![linea](immagini/linea.png)

## 2.3.4 Allocazione dinamica ed array

![linea](immagini/linea.png)

## 2.3.5 Rappresentzione degli array in memoria

![linea](immagini/linea.png)

## 2.3.6 Come non usare l'allocazione dinamica, 1

![linea](immagini/linea.png)

## 2.3.7 Come non usare l'allocazione dinamica, 2

![linea](immagini/linea.png)

## 2.4 ESERCIZI

  * Gli esercizi relativi alla prima lezione si trovano [qui](ESERCIZI.md)

