# 📚 Sprint 2-Tema2.03-MongoDB-Estructura de datos

Este repositorio contiene dos ejercicios prácticos desarrollados en MongoDB utilizando modelado NoSQL y colecciones JSON para una óptica en contexto colombiano.

---

## 📄 Descripción - Enunciado del ejercicio

### Ejercicio 1
Diseñar una base de datos MongoDB para una óptica "Cul d'Ampolla" desde el punto de vista del cliente, almacenando:
- Proveedores: Nombre, dirección, teléfono, fax, NIF
- Gafas: Marca, graduación, tipo/color de montura, color de cristales, precio
- Clientes: Datos personales, fecha registro, recomendaciones
- Empleados y ventas con fecha/hora

### Ejercicio 2
Rediseñar la base de datos con las gafas como elemento central, permitiendo visualizar qué clientes han comprado cada modelo.

---

## 💻 Tecnologías Utilizadas
- MongoDB
- JSON
- MongoDB Compass
- https://pandao.github.io/editor.md/en.html

---

## 📋 Requisitos
1. MongoDB 5.0+
2. MongoDB Compass
3. Visual Studio Code (opcional)
4. Node.js (opcional)

---

## 🛠️ Instalación
```bash
git clone https://github.com/nandox86/nandox86--Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git

# Importar colecciones
mongoimport --db optica --collection proveedores --file proveedores.json --jsonArray
mongoimport --db optica --collection gafas --file gafas.json --jsonArray
mongoimport --db optica --collection clientes --file clientes.json --jsonArray
mongoimport --db optica --collection empleados --file empleados.json --jsonArray
mongoimport --db optica --collection ventas --file ventas.json --jsonArray
mongoimport --db optica --collection compras_por_gafas --file compras_por_gafas.json --jsonArray

---

## ▶️ Ejecución
```javascript
// Buscar gafas de un proveedor
db.gafas.find({ "proveedor_id": ObjectId("6001f1d5e8c4a7b3c9d2e1f2") })

// Ver ventas de un empleado
db.ventas.find({ "empleado_id": ObjectId("6001f1d5e8c4a7b3c9d2e1f9") })

// Ver clientes por modelo de gafas
db.compras_por_gafas.find({ "modelo": "Google #" })

---

## 🌐 Despliegue
Proyecto educativo no diseñado para entorno de producción.

## 🤝 Contribuciones
```bash
git clone https://github.com/nandox86/nandox86--Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git
git checkout -b nombre-de-tu-rama
git add .
git commit -m "Descripción de los cambios"
git push origin nombre-de-tu-rama

Repositorio: [https://github.com/nandox86/nandox86--Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git](https://github.com/nandox86/nandox86--Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git)

---

### 📝 Notas Adicionales

- Estructura optimizada para análisis de ventas por modelo
- Ejercicios organizados en carpetas separadas

# ¡Gracias por revisar este proyecto! 😊
