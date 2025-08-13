# Lenguajes2025
trabajos lenguajes
## Descripción
Este repositorio tiene los ejemplos del pdf 'Flex__bizon',los ejemplos 1-1,1-2,1-3,1-4 y 1-5 ejecutables, hechos mediante flex, como analisador lexico, siguiendo pasos que dicen en el pdf.

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
