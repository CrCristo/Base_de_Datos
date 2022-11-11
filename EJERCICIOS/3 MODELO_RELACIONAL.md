Se desea diseñar una base de datos para almacenar y gestionar la información
empleada por una empresa dedicada a la venta de automóviles, teniendo en cuenta los
siguientes aspectos:
La empresa dispone de una serie de coches para su venta. Se necesita conocer la
matrícula, marca y modelo, el color y el precio de venta de cada coche.
Los datos que interesa conocer de cada cliente son el NIF, nombre, dirección, ciudad y
número de teléfono: además, los clientes se diferencian por un código interno de la
empresa que se incrementa automáticamente cuando un cliente se da de alta en ella. Un
cliente puede comprar tantos coches como desee a la empresa. Un coche determinado
solo puede ser comprado por un único cliente.
El concesionario también se encarga de llevar a cabo las revisiones que se realizan a
cada coche. Cada revisión tiene asociado un código que se incrementa automáticamente
por cada revisión que se haga. De cada revisión se desea saber si se ha hecho cambio de
filtro, si se ha hecho cambio de aceite, si se ha hecho cambio de frenos u otros. Los
coches pueden pasar varias revisiones en el concesionario

    USE tienda;

    /* esta nos permite modificar los datos de un obheto especifico
    UPDATE cliente
    SET nom_clie='Laura Pérez' WHERE clave_clie=23;*/

    /*Muestra toda la tabla de clientes
    SELECT * FROM cliente;*/

    /*esto saca la media de el precio de los productos o en general de una lista
    SELECT AVG(precio) FROM producto;*/

    /*ESTO nos cuenta el numnero de objetos que hay en una lista 
    SELECT COUNT(nom_prod) FROM producto; */

    /*Estp nos permite ver el producto con el precio más alto o bajo de la lista
    SELECT MAX(precio) FROM producto;
    SELECT MIN(precio) FROM producto; */

    /*empezamos a llenar la tabla de ventas
    INSERT INTO nota VALUES (1,93,89,2,NULL);
    ESTO es para agregar y modificar una enta
    UPDATE nota 
    INNER JOIN producto ON producto.clave_prod=nota.clave_prod1
    SET subtot=cant * precio WHERE folio=1;*/

    /*
    SELECT folio,nom_clie, clave_prod, nom_prod, cant, subtot
    FROM producto INNER JOIN nota ON nota.clave_prod1=producto.clave_prod 
    INNER JOIN cliente ON cliente.clave_clie=nota.clave_clie1;*/

    /*DROP elimina toda la base */
