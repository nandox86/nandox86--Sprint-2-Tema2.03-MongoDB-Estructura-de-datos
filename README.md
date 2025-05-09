
# <font>📚 Sprint 2-Tema2.03-MongoDB-Estructura de datos</font>

<font>Este repositorio contiene dos ejercicios prácticos desarrollados en MongoDB utilizando modelado NoSQL y colecciones JSON para una óptica en contexto colombiano.</font>

---

## <font>📄 Descripción - Enunciado del ejercicio</font>

### <font>Ejercicio 1</font>

<font>Diseñar una base de datos MongoDB para una óptica “Cul d'Ampolla” desde el punto de vista del cliente, almacenando:</font>

* <font>Proveedores: Nombre, dirección, teléfono, fax, NIF</font>
* <font>Gafas: Marca, graduación, tipo/color de montura, color de cristales, precio</font>
* <font>Clientes: Datos personales, fecha de registro, recomendaciones</font>
* <font>Empleados y ventas con fecha/hora</font>

### <font>Ejercicio 2</font>

<font>Rediseñar la base de datos con las gafas como elemento central, permitiendo visualizar qué clientes han comprado cada modelo.</font>

---

## <font>💻 Tecnologías utilizadas</font>

* <font>MongoDB</font>
* <font>JSON</font>
* <font>Brújula de MongoDB</font>
* [<font>https://pandao.github.io/editor.md/es.html</font>]

---

## <font>📋 Requisitos</font>

1. <font>MongoDB 5.0+</font>
2. <font>Brújula de MongoDB</font>
3. <font>Visual Studio Code (opcional)</font>
4. <font>Node.js (opcional)</font>

---

## <font>🛠️ Instalación</font>

<font>bash</font>  
<font>git clone</font>
[<font>https://github.com/nandox86/nandox86--Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git</font>]

 <font>Importar colecciones</font>.

<font>mongoimport —db optica —collection proveedores —file proveedores.json —jsonArray</font>  
<font>mongoimport —db optica —collection gafas —file gafas.json —jsonArray</font>  
<font>mongoimport —db optica —collection clientes —file clientes.json —jsonArray</font>  
<font>mongoimport —db optica —collection empleados —file empleados.json —jsonArray</font>  
<font>mongoimport —db optica —collection ventas —file ventas.json —jsonArray</font>  
<font>mongoimport —db optica —collection compras\_por\_gafas —file compras\_por\_gafas.json —jsonArray</font>

---

## <g-emoji><font>▶️</font></g-emoji><font>Ejecución</font>

<font>javascript</font>  
<font> Buscar gafas de un proveedor:</font>  
<font>db.gafas.find({ “proveedor\_id”: ObjectId(“6001f1d5e8c4a7b3c9d2e1f2”) })</font>

<font>// Ver ventas de un empleado</font>  
<font>db.ventas.find({ “empleado\_id”: ObjectId(“6001f1d5e8c4a7b3c9d2e1f9”) })</font>

<font>// Ver clientes por modelo de gafas</font>  
<font>db.compras\_por\_gafas.find({ “modelo”: “Google #” })</font>

---

## <font>🌐 Despliegue</font>

<font>Proyecto educativo no diseñado para entorno de producción.</font>

## <font>🤝 Contribuciones</font>

<font>git clone</font>. [<font>https://github.com/nandox86/nandox86--Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git</font>]
<font>git checkout -b nombre-de-tu-rama</font>  
<font>git add .</font>  
<font>git commit -m “Descripción de los cambios”</font>
<font>git push origin nombre-de-tu-rama</font>



<font>Repositorio:</font>[<font>https://github.com/nandox86/nandox86—Sprint-2-Tema2.03-MongoDB-Estructura-de-datos.git</font>]

---

 <font>📝 Notas adicionales</font>


* <font>Estructura optimizada para análisis de ventas por modelo.</font>
* <font>Ejercicios organizados en carpetas separadas</font>

# <font>¡Gracias por revisar este proyecto! 😊</font></react-app>
