# 🧮 Calculadora Java CI

Este es un proyecto de práctica diseñado para implementar un Pipeline de Integración Continua (CI) utilizando **GitHub Actions** en un proyecto Java simple (una calculadora con operaciones básicas).

## 🚀 Integración Continua (CI/CD)

Este repositorio está configurado con un flujo de trabajo de GitHub Actions que garantiza la calidad del código mediante la ejecución de los siguientes pasos cada vez que se realiza un `push` o un `Pull Request` a la rama `main`:

| Tarea | Estado del Workflow |
| :--- | :--- |
| **Compilación y Pruebas** | [Enlace a tu Pipeline de GitHub Actions - Reemplazar con el enlace real] |

## ⚙️ Estructura del Proyecto

El proyecto sigue una estructura simple de Java:

* **`.github/workflows/ci.yml`**: Contiene la definición del pipeline de CI de GitHub Actions (Compilación y Pruebas).
* **`src/`**: Contiene la lógica principal de la aplicación.
    * `Calculadora.java`: Clase que implementa las funciones de suma, resta, multiplicación y división.
* **`test/`**: Contiene las clases para la validación de la lógica.
    * `CalculadoraTest.java`: Contiene las pruebas unitarias (usando `assert`).
* **`lib/`**: Contiene librerías externas (como JUnit), aunque en este CI se usa solo código base para compilar.

## 💻 Funcionalidades de la Calculadora

La clase `Calculadora` proporciona los siguientes métodos estáticos:

| Método | Descripción | Parámetros |
| :--- | :--- | :--- |
| `sumar(a, b)` | Realiza la adición de dos números enteros. | `int a`, `int b` |
| `restar(a, b)` | Realiza la sustracción de dos números enteros. | `int a`, `int b` |
| `multiplicar(a, b)` | Realiza la multiplicación de dos números enteros. | `int a`, `int b` |
| `dividir(a, b)` | Realiza la división de dos números enteros. Lanza `ArithmeticException` si el divisor es cero. | `int a`, `int b` |
