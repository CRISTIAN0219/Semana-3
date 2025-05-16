# Estructuras Condicionales y Bucles en Python

Este repositorio contiene una guía práctica sobre el uso de estructuras condicionales (`if`, `else`, `elif`) y bucles (`for`, `while`) en Python, acompañada de ejemplos funcionales.

---

##  Estructura del proyecto

```
estructuras-condicionales-bucles/
├── ejemplos/
│   ├── if.py
│   ├── if_else.py
│   ├── if_elif_else.py
│   ├── for_basico.py
│   ├── for_variaciones.py
│   ├── while_basico.py
│   ├── while_iterador.py
│   ├── while_clave.py
│   ├── break_continue.py
├── README.md
```

---

## Contenido de los archivos

### Condicionales

#### `if`

```python
# ejemplos/if.py
edad = 18

if edad >= 18:
    print("Eres mayor de edad")
```

#### `if-else`

```python
# ejemplos/if_else.py
edad = 16

if edad >= 18:
    print("Eres mayor de edad")
else:
    print("Eres menor de edad")
```

#### `if - elif - else`

```python
# ejemplos/if_elif_else.py
edad = 18

if edad > 18:
    print("Eres mayor de edad")
elif edad == 18:
    print("Tienes 18 años")
else:
    print("Eres menor de edad")
```

### Bucles

#### Bucle `for`

```python
# ejemplos/for_basico.py
for i in "Python":
    print(i)
```

#### Variaciones de `for`

```python
# ejemplos/for_variaciones.py
texto = "Python"

# Reversa
for i in texto[::-1]:
    print(i)

# Saltos de dos en dos
for i in texto[::2]:
    print(i)

# Suma del 0 al 9
print(sum(i for i in range(10)))
```

#### Bucle `while`

```python
# ejemplos/while_basico.py
flag = "si"

while flag != "no":
    print("Hello world")
    flag = input("¿Deseas imprimir el mensaje otra vez?")
```

#### `while` con iterador

```python
# ejemplos/while_iterador.py
iterador = 0

while iterador < 5:
    print("El iterador es:", iterador)
    iterador += 1
```

#### Validación con intentos limitados

```python
# ejemplos/while_clave.py
intentos = 0
clave_correcta = "python123"
entrada = ""

while entrada != clave_correcta and intentos < 3:
    entrada = input("Introduce la contraseña: ")
    intentos += 1

if entrada == clave_correcta:
    print("¡Bienvenido!")
else:
    print("Demasiados intentos.")
```

### Break y Continue

```python
# ejemplos/break_continue.py

# Uso de break
contador = 1
while contador <= 10:
    if contador == 5:
        print("¡Encontré el número 5, saliendo!")
        break
    print("Número:", contador)
    contador += 1

# Uso de continue
contador = 0
while contador < 5:
    contador += 1
    if contador == 3:
        continue
    print("Contador:", contador)

# Mostrar solo impares
numero = 0
while numero < 10:
    numero += 1
    if numero % 2 == 0:
        continue
    print("Impar:", numero)
```

---

##  Instrucciones para subir a GitHub

1. Crea una carpeta llamada `estructuras-condicionales-bucles/`.
2. Dentro, crea una subcarpeta `ejemplos/`.
3. Crea los archivos `.py` y el `README.md` con el contenido proporcionado.
4. Inicia un repositorio Git y sube todo a GitHub:

```bash
cd estructuras-condicionales-bucles
git init
git add .
git commit -m "Primer commit"
git branch -M main
git remote add origin https://github.com/tuusuario/estructuras-condicionales-bucles.git
git push -u origin main
```

---

