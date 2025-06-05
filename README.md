# MisRecursosApp
```javascript
// Mostrar todos los recursos
db.recursos.find().pretty()
```
```javascript
// Cambiar estado de un libro
db.recursos.updateOne(
  { nombre: "The Hobbit" },
  { $set: { estado: "En progreso" } }
)
```
```javascript
// Eliminar un recurso por nombre
db.recursos.deleteOne({ nombre: "The Social Network" })
```
```javascript
// Filtrar por estado
db.recursos.find({ estado: "Terminado" })

// Filtrar por formato
db.recursos.find({ formato: "Libro" })

// Filtrar por plataforma
db.recursos.find({ plataforma: "Netflix" })

// Buscar por nombre (como barra de búsqueda)
db.recursos.find({ nombre: /hobbit/i })
```
