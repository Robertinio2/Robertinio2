Economia.tienda.mostrar(GuildId, Mensaje);
/*  
Esto sirve para mostrar la tienda de un servidor. 
GuildId => La Id del servidor
Mensaje => boolean (opcional) 
Por defecto es false. 
Si está en false, devolverá el Array de la tienda con cada Item.
Si está en true, devolverá un String de la tienda ya hecho.
*/
 
Economia.tienda.agregar(GuildId, Nombre, Descripción, Valor, Emoji);
/*
Esto sirve para agregar un objeto a la tienda.
GuildID => La id del servidor
Nombre => El nombre del objeto
Descripción => Una breve descripción del objeto
Valor => El valor del objeto (Tiene que ser un Número)
Emoji => Emoji de Discord
*/
 
Economia.tienda.sacar(GuildId, Número);
/*
Esto sirve para quitar un objeto de la tienda.
GuildId => La Id del servidor.
Número => El número en el cual el objeto se encuentra en la tienda.
*/
 
Economia.tienda.comprar(GuildId, UserId, Número);
/*
Esto sirve para que un usuario compre un objeto de la tienda (Usando el dinero en mano del Usuario).
GuildId => La Id del servidor.
UserId => La Id del usuario.
Número => El número en el cual el objeto se encuentra en la tienda.
*/
 
Economia.dinero.mostrar(GuildID, UserID);
/*
Devuelve cuanto dinero tiene un usuario en un objeto.
GuildId => La id del servidor
UserId => La id del usuario
*/
 
Economia.dinero.agregar(GuildID, UserID, Username, Cantidad, Banco);
/*
Esto sirve para agregar dinero a un usuario.
GuildId => La id del servidor en el cual está el usuario
UserId => La id del usuario al cual se le agregará la cantidad de dinero especificada
Username => El nombre del usuario al cual se le agregará la cantidad de dinero especificada
Cantidad => La cantidad de dinero a agregar
Banco => boolean (opcional)
Por defecto: false
Si está en false, le agregará el dinero en el dinero en mano del usuario.
Si está en true, le agregará el dinero en el banco del usuario.
 
Devuelve un objeto con el dinero en mano y en el banco del usuario actualizado.
*/
 
Economia.dinero.sacar(GuildID, UserID, Username, Cantidad, Banco);
/*
Esto sirve para sacarle dinero a un usuario
GuildId => La id del servidor en el cual está el usuario
UserId => La id del usuario al cual se le quitará la cantidad de dinero
Username => El nombre del usuario al cual se le quitará la cantidad de dinero
Cantidad => La cantidad de dinero a sacar
Banco => boolean (opcional)
Por defecto: false
Si está en false, le quitará el dinero en el dinero en mano del usuario.
Si está en true, le quitará el dinero en el banco del usuario.
 
Devuelve un objeto con el dinero en mano y en el banco del usuario actualizado.
*/
 
Economia.dinero.depositar(GuildID, UserID, Username, Cantidad)
/*
Deposita una Cantidad de dinero en mano del Usuario al banco del usuario.
GuildId => La id del servidor en el cual está el usuario.
UserId => La id del usuario.
Username => El nombre del usuario.
Cantidad => La cantidad que se quiere depositar en el banco.
En caso de que se quiera depositar todo el dinero que tiene actualmente al banco,
escribir "todo" o "all".
 
Devuelve un objeto con el dinero en mano y en el banco del usuario actualizado.
*/
 
Economia.dinero.retirar(GuildID, UserID, UserName, Cantidad)
/*
Retira dinero del Banco del usuario y lo obtiene como dinero en mano del usuario.
GuildId => La id del servidor en el cual está el usuario.
UserId => La id del usuario.
Username => El nombre del usuario.
Cantidad => La cantidad que se quiere retirar del banco.
En caso de que se quiera retirar todo el dinero que tiene actualmente en el banco,
escribir "todo" o "all".
*/
 
 
Economia.dinero.leaderboard(GuildId);
/*
Devuelve un Array con el ranking de las personas con más dinero.
GuildId => La id del servidor
*/
 
Economia.dinero.reiniciar(GuildID, UserID, UserName);
/*
Reinicia el dinero del usuario.
GuildId => La id del servidor en el cual está el usuario.
UserId => La id del usuario.
Username => El nombre del usuario.
*/Economia.inventario.mostrar(GuildId, UserId, Mensaje);
/*
Sirve para ver los objetos comprados por el Usuario.
GuildId => La id del servidor en el cual está el usuario.
UserId => La id del usuario.
Mensaje => boolean (opcional) 
Por defecto es false. 
Si está en false, devolverá el Array del inventario del usuario con sus respectivos objetos.
Si está en true, devolverá un String del inventario ya hecho.
*/
Economia.inventario.agregar(GuildId, UserId, Número);
/*
Agrega un item de la tienda al inventario del usuario.
GuildId => La id del servidor en el cual está el usuario.
UserId => La id del usuario.
Número => El número en el cual el objeto se encuentra en la tienda.
*/
Economia.inventario.sacar(GuildId, UserId, Número);
/*
Remueve un item del inventario del usuario.
GuildId => La id del servidor en el cual está el usuario.
UserId => La id del usuario.
Número => El número en el cual el objeto se encuentra en el inventario del usuario.
*/
 
