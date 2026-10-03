# Estructura de Datos — UNIMINUTO 2026

Repositorio para los laboratorios y actividades de la asignatura **Estructura de Datos** (NRC: 90547) en la Corporación Universitaria Minuto de Dios — Sede Ciudad Bolívar.

---

## 📌 Información General

* **Institución:** Corporación Universitaria Minuto de Dios – UNIMINUTO
* **Asignatura:** Estructura de Datos
* **NRC:** 90547
* **Docente:** Edilberto Ramirez Rivera
* **Ubicación:** Ciudad Bolívar – 2026

---

## 👥 Integrantes

* **Oscar Stiven Avila Nomesque** — ID: 1045928
* **David Santiago Borda Jimenez** — ID: 1095539
* **Andres Sebastian Reina Yazo** — ID: 1094995

---

## 📚 Conceptos Básicos

### 1. Pila (*Stack*)
Es una estructura de datos que funciona bajo el principio **LIFO** (*Last In, First Out* o "Último en entrar, primero en salir"). Se asemeja a una pila de platos: el último plato que pones en la cima es el primero que debes retirar.

### 2. Cola (*Queue*)
Es una estructura de datos que funciona bajo el principio **FIFO** (*First In, First Out* o "Primero en entrar, primero en salir"). Funciona como una fila en un supermercado: la primera persona en llegar es la primera en ser atendida.

---

## 💻 Códigos Implementados

### 1. AlmacenListasEnlazadas
**Idea Principal:** 
La idea principal de este código es implementar tanto una cola como una pila dinámicas utilizando listas enlazadas (basadas en una clase `Nodo`). 
* Se utiliza una clase `ColaCamiones` para registrar los camiones que llegan a un muelle (insertando nodos al final) y atenderlos (removiendo nodos del frente)
* Se implementa una clase `PilaCajas` para apilar cajas en la parte superior (el tope) y procesarlas retirándolas de ese mismo extremo.
### 2. CentroLogisticaGalactica
**Idea Principal:** 
La idea principal de este código es simular un centro logístico combinando el uso de un arreglo de tamaño fijo para una cola y una estructura de nodos enlazados para una pila
* Utiliza un arreglo circular llamado `muelleDrones` que funciona como una cola con una capacidad máxima de 5 espacios para gestionar los drones que llegan a atracar
* Al llamar al método `procesarDron()`, el sistema retira un dron de la cola, "descarga" su caja de suministros y la almacena en una pila basada en nodos llamada `topeAlmacen` utilizando el método `pushAlmacen`
