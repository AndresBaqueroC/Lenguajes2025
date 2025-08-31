# Lenguajes2025
trabajos lenguajes
## Descripción
Este repositorio tiene los ejercicios realizados en el primer corte de la ametia de lenguajes. Los trabajos solicitadops como del pdf 'Flex__bizon',los ejemplos 1-1,1-2,1-3,1-4 y 1-5 ejecutables, hechos mediante flex, como analisador lexico, siguiendo pasos que dicen en el pdf.  Autoamtas usando flex, bison, implementacion en py, y antlr calculadora.

## Contenido
- Taller 1
- Taller 2
- Taller 3
- Taller antl4 Calculadora

# Taller ANTLR Calculadora 
### Descripcion:
Por cuestion de orden mas que nada lo separe por carpetas, una para java y la otra para PYTHON,por eso para este caso al ejecutar en py uso un ambiete o entorno virtual.
### Instrucciones para ejecurtar
1. Principalmente despues de descargar el zip, descomprimir y mandar la carpeta a ruta donde este el antlr-4..complete.jar.  En mi caso era
```bash
cd Escritorio/antlr-4.13.0-complete
```
2. En este 2 es poner la carpeta de paso CalculadoraEjerciciosantlr en esa ruta anterior.
 ```bash
mv CalculadoraEjerciciosantlr/ antlr-4.13.0-complete/CalculadoraEjercicios/
 ```
3. Decidimos cual queremos ejecutary ponemos la ruta
   **Caso java**
   ```bash
   cd CalculadoraEjerciciosantlr/javaCalcula
   ```
   El zip ya tiene los analizadores pero en caso tal es:
   ```bash
   antlr4 -no-listener -visitor LabeledExpr.g4  #Tener en cuenta que ya tiene el alias
   ```
   Para la compilacion de los archivos Java seria:
   ```bash
   javac -cp ".::/usr/local/lib/antlr-4.13.0-complete.jar" *.java
   ```
   para ejecutar:
   ```bash
   java -cp ".::/usr/local/lib/antlr-4.13.0-complete.jar" Calc test.txt
   ```
   **Caso PYTHON**
   ```bash
   cd ~/Escritorio/antlr-4.13.0-complete/Calculadoraejercicios/python/
   ```
   Generar analizadores Python
   ```bash
   antlr4 -Dlanguage=Python3 -no-listener -visitor LabeledExpr.g4
   ```
   **Ojo como estan en carpetas y en este caso el entorno virtual porque python por lo general ya viene preinstalado en ubuntu(mi distribuidor) al usar un entorno virtual pues deja instalar mas dependencias sin errores**
   ```bash
   python3 -m venv antlr_env
   source antlr_env/bin/activate
   pip install antlr4-python3-runtime
   ```
   y ya ejecutar
   ```bash
   python Calc.py test.txt
   ```

# Taller 3
### Descripcion:
Implementacion de ejercicio propuesto de automata finito determinista, en el zip de Automata cuenta con codigo ejecutable en Python y implementacion en Bison y flex, obviamente con logica para la parte lexica y del parsel pàra que funcione.  No estoy seguro de si deberia documentar los codigos asi que comence a hacerlo por si acaso

####Reglas
Q=q1,q2,q3,q4
E=0,1
q0= q1
F=q3
(q1,0)=q4
(q1,1)=q2
(q2,0)=q2
(q2,1)=q3
(q4,1)=q4
(q4,0)=q4
(q3,0)=q3
(q3,1)=q3

Imagen de Guia Visual de programa Jflap

#### cadena: 1000001

<img width="674" height="467" alt="image" src="https://github.com/user-attachments/assets/bba26dfe-ab5c-46f4-bdb5-07c02581ac32" />

#### Cadena:1000001

<img width="674" height="467" alt="image" src="https://github.com/user-attachments/assets/9b332163-780a-4613-8b35-b47dda270b8a" />

### Ejecucion en C y Py

<img width="1822" height="206" alt="image" src="https://github.com/user-attachments/assets/01259fba-bc5b-4a46-b345-6e5e3353944e" />


# Taller2
## Descripcion: 
En este 2 taller contiene ejercicios propuestos por docente de gramatica, implementacion de comportamiento de gramaticas L(G1), L(G2), L(G3), L(G4), L(G5). Implementadas en **C y Python**, donde acepten cualquier archivo txt, para hacer las pruebas respectivas.

## Contenido:
### Gramatica 1:
Primera gramatica era practicamente un polindromo de numeros binarios, osea que se lea de igual manera tanto derecho como a la inversa.
<img width="1462" height="303" alt="image" src="https://github.com/user-attachments/assets/4f56dd1f-70fc-4689-aa95-3011cea83c48" />

### Gramatica 2:
La segunda gramtica era que su abecedario era (a,b), pero con condicion de que a podia ser de 0 a muchos a* y b minimo tenia que haber 1 **b+**.  a*b+=a+1
En este ejemplo tuve un problema en la parte lexica osea flex, si lo arreglo cambio esto si no puesss.
<img width="1317" height="341" alt="image" src="https://github.com/user-attachments/assets/1692ce6b-c32a-41e4-90ba-51056c58b284" />


### Gramatica 3:
La tercera era al parecida a la segunda gramatica con el ligero cambio de que tanto a como b tenian que se de 1 a varios osea minimo 1 de cada 1 y siempre tenia que haber un b mas que a. **a+ b+=a+1**  
<img width="1483" height="395" alt="Captura desde 2025-08-12 21-31-25" src="https://github.com/user-attachments/assets/65c2376d-8926-4910-8880-232a325992b6" />

### Gramatica 4:
Esta tercera gramatica solo aceptaba abb o ab.  **a+b+**
<img width="1462" height="303" alt="Captura desde 2025-08-12 21-34-33" src="https://github.com/user-attachments/assets/8b71ecfa-ab84-4777-8746-5f0222c70ccc" />

### Gramatica 5:
El quinto la condicion principal es que iniciara con a y terminara en b minimo 1 de cada uno osea **a+ b+**, pero tambien con una variante (ab)* pues podria ser de 0 a verios.
<img width="1462" height="303" alt="Captura desde 2025-08-12 21-35-11" src="https://github.com/user-attachments/assets/3fe8f76b-4c85-402f-95d0-bd6b72ccee45" />


### Taller 1
## Contenido
- ejemplo 1-1
- ejemplo 1-2
- ejemplo 1-3
- ejemplo 1-4
- ejemplo 1-5
(solucion de ejercicios propuestos docente)
- Sejercicio 
- Sejercicio6

## Como ejecutar?
- Principalmente tener Flex y Bison: en caso de no:  **'sudo apt install flex bison'** 
- Abrir terminal, llevar a direccion de carpetas cd 'ruta'.

# para ejecutar './nombre definido':
- 1-1:'**./contador** ' 
- 1-2:'**./traducir.l**'
- 1-3:'**./tokens.l**'
- 1-4:'**./Ejemplo1-4.l**'
- 1-5:'**./calculadora**'
- Sejercicio:'**./calculadoraexa**'
- Sejercicio6:'**./a.out**':flex   '**./Ccontador**':C

