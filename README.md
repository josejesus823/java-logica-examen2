
# 🛠️ Lista de Errores y Correcciones en el Código Java

A continuación se presenta una lista de errores identificados en el código Java junto con sus respectivas correcciones. Esto te servirá como guía para evitar errores comunes durante el desarrollo. ✅

---

## ❌ Error 1: Scanner mal escrito
- ❗ `scanner` estaba en minúscula y faltaba `System.in`
- ✅ **Corrección:** `Scanner sc = new Scanner(System.in);`

---

## ❌ Error 2: Problemas con `print` y `nextLine`
```java
System.out.print"Ingrese el nombre del programador: ");
nombreProgramador = sc.nextline()
```
- ❗ Falta paréntesis inicial en `print`
- ❗ `nextline()` debe ser `nextLine()`
- ❗ Falta `;` al final
- ✅ **Corrección:**
```java
System.out.print("Ingrese el nombre del programador: ");
nombreProgramador = sc.nextLine();
```

---

## ❌ Error 3: Nombre de variable incorrecto
```java
System.out.print("Ingrese el correo electrónico: ")
correo = scanner.nextLine();
```
- ❗ Falta `;` en el `print`
- ❗ `scanner` debe ser `sc`
- ✅ **Corrección:**
```java
System.out.print("Ingrese el correo electrónico: ");
correo = sc.nextLine();
```

---

## ❌ Error 4: Nombre de objeto `Scanner` incorrecto
```java
ciudad = leer.nextLine();
```
- ❗ `leer` debe ser `sc`
- ✅ **Corrección:** `ciudad = sc.nextLine();`

---

## ❌ Error 5: Falta punto y coma
```java
System.out.print("Ingrese el país: ")
```
- ❗ Falta `;`
- ✅ **Corrección:** `System.out.print("Ingrese el país: ");`

---

## ❌ Error 6: Falta punto y coma
```java
System.out.print("Ingrese el tipo de contrato (Fulltime/Parttime/Freelance): ")
```
- ❗ Falta `;`
- ✅ **Corrección:** `System.out.print("Ingrese el tipo de contrato (Fulltime/Parttime/Freelance): ");`

---

## ❌ Error 7: Notación decimal incorrecta
```java
tarifaBase = 50,0,0;
```
- ❗ Se usaron comas en lugar de un punto
- ✅ **Corrección:** `double tarifaBase = 50.0;`

---

## ❌ Error 8: Falta punto y coma
```java
System.out.println("\nTarifa final por hora calculada: $" + tarifaHoraFinal)
```
- ❗ Falta `;`
- ✅ **Corrección:** `System.out.println("\nTarifa final por hora calculada: $" + tarifaHoraFinal);`

---

## ❌ Error 9: Uso incorrecto de Scanner y falta de `;`
```java
System.out.print("Cliente 1: ")
cliente1 = sc.nex();
```
- ❗ Falta `;`
- ❗ Método incorrecto: `nex()` → debe ser `nextLine()`
- ✅ **Corrección:**
```java
System.out.print("Cliente 1: ");
cliente1 = sc.nextLine();
```

---

## ❌ Error 10: Falta punto y coma
```java
System.out.print("Cliente 2: ")
```
- ❗ Falta `;`
- ✅ **Corrección:** `System.out.print("Cliente 2: ");`

---

## ❌ Error 11: Scanner mal usado y falta de punto y coma
```java
System.out.print("Cliente 3: ")
cliente3 = sc.nex();
```
- ❗ Falta `;`
- ❗ `nex()` incorrecto, se recomienda `nextLine()`
- ✅ **Corrección:**
```java
System.out.print("Cliente 3: ");
cliente3 = sc.nextLine();
```

---

## ❌ Error 12, 13 y 14: Líneas comentadas
```java
//horasProyecto1 = sc.nextInt();
//horasProyecto2 = sc.nextInt();
//horasProyecto3 = sc.nextInt();
```
- ❗ Están comentadas, no se ejecutan
- ✅ **Corrección:** Quitar los `//` al inicio

---

## ❌ Error 15, 16 y 17: Nombres mal escritos
```java
pagoProyecto1 = (horasProyec1 * tarifaHoraFinal) + bonusCliene1;
pagoProyecto2 = (horasProyecto2 * tarifaHoraFnal) + bonusCliene2;
pagoProyecto3 = (horasProyecto3 * tarifaHoraFinal) + bonusCliene3;
```
- ❗ Variables con errores tipográficos
- ✅ **Correcciones:**
```java
pagoProyecto1 = (horasProyecto1 * tarifaHoraFinal) + bonusCliente1;
pagoProyecto2 = (horasProyecto2 * tarifaHoraFinal) + bonusCliente2;
pagoProyecto3 = (horasProyecto3 * tarifaHoraFinal) + bonusCliente3;
```

---

## ❌ Error 18: Operador mal usado
```java
subtotal ==== pagoProyecto1 + pagoProyecto2 + pagoProyecto3;
```
- ❗ Cuatro signos de igual (`====`)
- ✅ **Corrección:** `subtotal = pagoProyecto1 + pagoProyecto2 + pagoProyecto3;`

---

## ❌ Error 19: Falta de import
```java
LocalDate fechaActual = LocalDate.now();
```
- ❗ Falta importar `java.time.LocalDate`
- ✅ **Corrección:** `import java.time.LocalDate;`

---

## ⚠️ Advertencia 20: Variable no usada
- ❗ Se declaró una variable `edad`, pero no se utilizó ni se imprimió.
- ✅ **Recomendación:** Usar `System.out.println("Edad: " + edad);` si se desea mostrar

---

🧠 **Consejo final:** Revisa siempre la consola por errores de compilación. Java es estricto con la sintaxis, especialmente con los métodos en mayúscula, punto y coma `;`, y los nombres de métodos de `Scanner`.
