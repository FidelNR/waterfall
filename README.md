# Resumen sobre solución del *Waterfall*

### Promesas Paralelas:
- Se presentó cómo realizar **múltiples solicitudes** de datos en paralelo utilizando promesas.
- La idea es no esperar a todas las solicitudes antes de actualizar el estado, sino actualizar el estado independientemente para cada solicitud a medida que se completan.

### Proveedores de Datos:
- Se introdujo el concepto de *proveedores de datos* para abstraer la obtención de datos en un solo lugar de la aplicación.
- Los proveedores de datos utilizan el contexto de *React* para proporcionar datos a componentes secundarios sin necesidad de pasar props manualmente.
- Esto ayuda a evitar la perforación de props y mejora la legibilidad y la organización del código.

### Recuperación de Datos Antes de React:
- Se discutió cómo mover las llamadas de recuperación de datos fuera del ciclo de vida de *React* puede mejorar el rendimiento al evitar las **cascadas de solicitudes**.
- Al mover las llamadas de recuperación antes de que *React* comience a renderizar componentes, se pueden obtener los datos de manera más eficiente y sin afectar el **rendimiento de la aplicación**.

### Bibliotecas y Suspense:
- Se mencionó que si bien se pueden utilizar bibliotecas como **Axios o SWR** para manejar las solicitudes de datos, los principios fundamentales de obtención de datos en *React* **siguen siendo los mismos**.
- Se señaló que el *Suspense* para la obtención de datos todavía está en **fase experimental** en *React*, pero puede ser una herramienta útil para manejar el estado de carga de manera más elegante en el futuro.