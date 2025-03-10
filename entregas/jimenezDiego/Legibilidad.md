# Legibilidad

## Códigos

| Retos       | Enlace |
|------------------|--------|
| **SpotifyApp** | [Código](https://github.com/diegojiimenez/24-25-EDA1/blob/reto-004/entregas/jimenezdiego/reto-004/reto004/SpotifyApp.java) |
| **SistemaCalificación**  | [Código](https://github.com/diegojiimenez/Sistema-de-Calificacion/blob/main/SistemaCalificacion.java) |
| **LibraryManager** | [Código](https://github.com/SantiGT1503/23-24-eda2-ep/blob/main/entregas/ExamenParcial/v003/src/LibraryManager.java) |
| **OrdenadorBaraja** | [Código](https://github.com/diegojiimenez/23-24-eda2/blob/main/entregas/DiegoJimenez/reto007/OrdenadorDeBaraja.java) |
| **LibraryManager** | [Código](https://github.com/diegojiimenez/23-24-eda2/blob/main/entregas/DiegoJimenez/reto003/v01/Documento.java) |
| **AspiradoraRobotica** | [Código](https://github.com/diegojiimenez/Aspiradora-Robotica/blob/main/AspiradoraRobotica.java) |
| **Dietas** | [Código](https://github.com/diegojiimenez/23-24-eda2/blob/main/entregas/DiegoJimenez/reto002/Day.java) |



### 1. Nombrado
|||
|-|-|
|Elige una palabra para un concepto abstracto y aferrarte a él. Algunos métodos usan añadir y otros agregar |[Ver Línea](https://github.com/diegojiimenez/24-25-EDA1/blob/2b35ae6a5cde789ed2b096b6b321d802acbf039c/entregas/jimenezdiego/reto-004/reto004/SpotifyApp.java#L159)|

### 2. Comentarios

|||
|-|-|
|Comentarios que no aportan nada al código ya que es obvio.| [Ver Línea](https://github.com/diegojiimenez/Sistema-de-Calificacion/blob/44c268a29ed87817470bdbb3c88ccc3dc3a24ee6/SistemaCalificacion.java#L93)|
### 3. Formato
|||
|-|-|
|Inconsistencia en el uso de nombres de variables. Deberían seguir el mismo formato que books, authors y keywords. Un mejor nombre sería authorRelations y keywordRelations para mantener la coherencia en camelcase.| [Ver Línea](https://github.com/SantiGT1503/23-24-eda2-ep/blob/74e5fbf697808aeea180a41f2f4155bc5c13b478/entregas/ExamenParcial/v003/src/LibraryManager.java#L13)|

### 4. Estandares
|||
|-|-|
|No sigue los estándares de la industria. Uso de operadores de comparación con char. Si getPalo() devuelve un string, se debería usar compareTo() en lugar de < y == para evitar errores de comparación.| [Ver Línea](https://github.com/diegojiimenez/23-24-eda2/blob/1df428be0b36bdfdd884fa2a2b46fa48f15df8c1/entregas/DiegoJimenez/reto007/OrdenadorDeBaraja.java#L46)|

### 5. Consistencia
|||
|-|-|
|El método addPalabraClave(String palabraClave) convierte la palabra clave a minúsculas (palabraClave.toLowerCase()) antes de agregarla a la lista, pero no hay ninguna indicación de que otras propiedades del documento, como el título o el tipo de documento, sigan la misma convención.| [Ver Línea](https://github.com/diegojiimenez/23-24-eda2/blob/1df428be0b36bdfdd884fa2a2b46fa48f15df8c1/entregas/DiegoJimenez/reto003/v01/Documento.java#L48)|

### 6. Codigo muerto
|||
|-|-|
|El decremento de bateria (bateria--;) ocurre dos veces en moverAspiradora() por lo que la segunda vez está de más.| [Ver Línea](https://github.com/diegojiimenez/Aspiradora-Robotica/blob/05c5fa5049514350418f64c08467273c6e1b7123/AspiradoraRobotica.java#L62)|

### 7. DRY
|||
|-|-|
|Los métodos updateIntake y deleteIntake repiten una estructura de búsqueda similar en intakeList. Ambos iteran sobre la lista para encontrar una ingesta con un nombre específico y realizan una acción (setName o remove).| [Ver Línea](https://github.com/diegojiimenez/23-24-eda2/blob/1df428be0b36bdfdd884fa2a2b46fa48f15df8c1/entregas/DiegoJimenez/reto002/Day.java#L64)|

### 8. YAGNI
|||
|-|-|
|La clase Materia solo almacena datos sin agregar ninguna lógica útil. Actualmente, no hace más que actuar como un simple contenedor de información, y no se usa ninguna funcionalidad adicional que justifique su existencia en lugar de simplemente usar un Map<String, Double> en la clase Estudiante.| [Ver Línea](https://github.com/diegojiimenez/Sistema-de-Calificacion/blob/44c268a29ed87817470bdbb3c88ccc3dc3a24ee6/SistemaCalificacion.java#L5)|