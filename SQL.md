Se eligieron estos tipos de datos por su simplicidad y utilidad: int para los id porque son números únicos y
fáciles de manejar, varchar para Nombre y Correo ya que son textos de longitud variable, decimal(10,2) para
Monto y Saldo porque representan dinero y necesitan precisión, y date para Fecha porque permite guardar
fechas correctamente; en general son tipos básicos que hacen la base de datos fácil de usar.

Create database Gastos;

Create table Usuario (
id int Primary Key,
Nombre varchar(50),
Correo varchar(50)
);

Use Gastos;

Create table Ingreso (
id int Primary Key,
Monto decimal(10,2),
Fecha date,
id_usuario int
);

Create table Egreso (
id int Primary Key,
Monto decimal(10,2),
Fecha date,
id_usuario int
);

Create table Balance (
id int Primary Key,
Saldo decimal(10,2),
id_usuario int
);
