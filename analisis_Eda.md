1. title 📝 (Título de la película)
Nulos: 0 (0.00%) ✅
Valores Únicos: Varía por título
Tipo de Dato: object
Transformaciones: Ninguna. ✅
Tratamiento de Nulos: No aplica✅
Duplicados: Ninguno❓

2. **Production company** 🏢 (Compañía de producción)
Nulos: 40 (9.26%) ⚠️
Valores Únicos: Lista de nombres
Tipo de Dato: object
**Transformaciones:** **explode para separar compañías en múltiples filas. Quedarse con el primer elemento de la lista**
**Tratamiento de Nulos**: **segun corresponda**
Duplicados: Verificar después del explode

3. **Release date** 📅 (Fecha de estreno)
Nulos: 1 (0.23%) ⚠️
Unique: Varía por fecha
Valores Únicos: Diferentes fechas
Tipo de Dato: object (listas)
Transformaciones: 
**-Crear una nueva columna con el lugar de estreno**
**-Quedarse con el primer elemento de la lista**
**-Crear una nueva columna con el lugar de estreno si está presente en el formato (dentro de paréntesis)**
**-Convertir la fecha a formato datetime**
**Tratamiento de Nulos: Gestionar nulos**
Duplicados: Revisar tras la transformación

4. Running time ⏱️ (Duración en texto)
Nulos: 10 (2.31%) ⚠️
Unique: Varía por duración
Valores Únicos: Diferentes duraciones
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: gestionar
Duplicados: No aplica

5. **Country**🌍 (País de origen)
Nulos: 4 (0.93%) ⚠️
Unique: Varía por país
Valores Únicos: Lista de países
Tipo de Dato: object
**Transformaciones:** Explode (dividir en varias filas si contiene múltiples países)
**Tratamiento de Nulos:** gestionar
Duplicados: Verificar después del explode

6. **Language** 🗣️ (Idioma)
Nulos: 2 (0.46%) ⚠️
Unique: Varía por idioma
Valores Únicos: Lista de idiomas
Tipo de Dato: object (tiene listas)
**Transformaciones:** explode para separar idiomas en múltiples filas
**Tratamiento de Nulos:** gestionar 
Duplicados: Verificar después del explode

7. **Running time (int)** ⏱️ (Duración en minutos)
Nulos: 10 (2.31%) ⚠️
Unique: Varía por duración
Valores Únicos: Diferentes duraciones
Tipo de Dato: float64
**Transformaciones:** eliminar (int) del titulo
**Tratamiento de Nulos:** gestionar
Duplicados: Ninguno

8. **Budget (float)** 💵 (Presupuesto en millones)
Nulos: 159 (36.81%) ⚠️
Unique: Varía por presupuesto
Valores Únicos: Diferentes valores monetarios
Tipo de Dato: float64
**Transformaciones:** eliminar float del titulo, ver la moneda y si hay que convertir el numero 
**Tratamiento de Nulos:** gestionar
Duplicados: Revisar después del tratamiento de nulos

9. **Box office (float)** 💰 (Ingresos en taquilla en millones)
Nulos: 77 (17.82%) ⚠️
Unique: Varía por ingresos
Valores Únicos: Diferentes valores monetarios
Tipo de Dato: float64
**Transformaciones:** eliminar float del titulo, ver la moneda y si hay que convertir el numero 
**Tratamiento de Nulos:** gestionar
Duplicados: Revisar después del tratamiento de nulos

10. **Release date (datetime)** 📅 (Fecha de estreno en formato datetime)
Nulos: 4 (0.93%) ⚠️
Unique: Varía por fecha
Valores Únicos: Diferentes fechas
Tipo de Dato: object
**Transformaciones:** eliminar datetime del titulo
**Tratamiento de Nulos:** gestionar lo snulos como una nueva categori????
Duplicados: Verificar tras la transformación

11. **imdb** ⭐ (Puntuación en IMDb)
Nulos: 16 (3.70%) ⚠️
Unique: Varía por puntuación
Valores Únicos: Diferentes valores de puntuación
Tipo de Dato: float64
Transformaciones: Ninguna
**Tratamiento de Nulos:** gestionar fillna 0?
Duplicados: Ninguno

12. metascore 🎯 (Puntuación de Metascore)
Nulos: 149 (34.49%) ⚠️
Unique: Varía por puntuación
Valores Únicos: Diferentes valores de puntuación
Tipo de Dato: float64
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

13. rotten_tomatoes 🍅 (Puntuación de Rotten Tomatoes)
Nulos: 71 (16.44%) ⚠️
Unique: Varía por puntuación
Valores Únicos: Diferentes valores de puntuación
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

14.**Directed by** 🎬 (Director/es de la película)
Nulos: 1 (0.23%) ⚠️
Unique: Varía por director
Valores Únicos: Diferentes nombres
Tipo de Dato: object (lista)
**Transformaciones:** Quedarse con el primer elemento de la lista, quitar las categorias que no vamos a usar 
**Tratamiento de Nulos:** gestionar
Duplicados: Verificar después de la transformación

15. **Produced by** 🏗️ (Productor/es de la película)
Nulos: 10 (2.31%) ⚠️
Unique: Varía por productor
Valores Únicos: Diferentes nombres
Tipo de Dato: object (lista)
**Transformaciones:** Quedarse con el primer elemento de la lista
**Tratamiento de Nulos:** gestionar
Duplicados: Verificar después de la transformación

16. Written by ✍️ (Guionista/s de la película)
Nulos: 229 (53.01%) ⚠️
Unique: Varía por guionista
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

17. **Based on** 📚 (Basado en)
Nulos: 221 (51.16%) ⚠️
Unique: Varía por obra
Valores Únicos: Diferentes títulos o nombres
Tipo de Dato: object (lista)
**Transformaciones:** 
**Convertir lista  quedándose con el primer elemento**
**-Limpieza de caracteres innecesarios**
**Tratamiento de Nulos: gestionar**
Duplicados: Verificar tras la transformación

18. Starring 🎭 (Protagonistas)
Nulos: 34 (7.87%) ⚠️
Unique: Varía por actores
Valores Únicos: Lista de actores
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

19. Music by 🎶 (Compositor/es de la banda sonora)
Nulos: 10 (2.31%) ⚠️
Unique: Varía por compositor
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

20. **Distributed by** 🚚 (Distribuidora/s)
Nulos: 3 (0.69%) ⚠️
Unique: Varía por distribuidora
Valores Únicos: Diferentes nombres
Tipo de Dato: object (listas)
**Transformaciones:** Quedarse con el primer elemento de la lista
**Tratamiento de Nulos:** gestionar
Duplicados: Verificar tras la transformación

21. Budget 💵 (Presupuesto en texto)
Nulos: 156 (36.11%) ⚠️
Unique: Varía por presupuesto
Valores Únicos: Diferentes valores monetarios en texto
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

22. Box office 💰 (Ingresos en taquilla en texto)
Nulos: 73 (16.90%) ⚠️
Unique: Varía por ingresos
Valores Únicos: Diferentes valores monetarios en texto
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

23. Story by 📖 (Historia de la película)
Nulos: 293 (67.82%) ⚠️
Unique: Varía por autor
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

24. Narrated by 🎙️ (Narrador/es de la película)
Nulos: 377 (87.27%) ⚠️
Unique: Varía por narrador
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

25. Cinematography 🎥 (Cinematógrafo/s)
Nulos: 90 (20.83%) ⚠️
Unique: Varía por cinematógrafo
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

26. Edited by ✂️ (Editor/es)
Nulos: 37 (8.56%) ⚠️
Unique: Varía por editor
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

27. Screenplay by 📝 (Guión de la película)
Nulos: 241 (55.79%) ⚠️
Unique: Varía por guionista
Valores Únicos: Diferentes nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

28. Production companies 🏢 (Lista de compañías de producción)
Nulos: 393 (90.97%) ⚠️
Unique: Varía por compañía
Valores Únicos: Lista de nombres
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

29. Adaptation by 📚 (Adaptación por)
Nulos: 431 (99.77%) ⚠️
Unique: Varía por autor
Valores Únicos: 1 único valor
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

30. Traditional 📜 (Versión tradicional)
Nulos: 431 (99.77%) ⚠️
Unique: Varía por versión
Valores Únicos: 1 único valor
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica

31. Simplified ✍️ (Versión simplificada)
Nulos: 431 (99.77%) ⚠️
Unique: Varía por versión
Valores Únicos: 1 único valor
Tipo de Dato: object
Transformaciones: ***Eliminar columna***
Tratamiento de Nulos: No aplica
Duplicados: No aplica