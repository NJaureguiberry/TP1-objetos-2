1) Elijo la opción 1 ya que cre el objeto rectangulo a partir de la clase "Rectangulo" y posterior a eso inicializa las 4 variables detalladas en el enunciado.
     En contra parte la opción 2 no respeta las variables ya definidas , lo cual llevaría a un error en el código.
     
2) Elijo la opción 2 ya que por medio del buen uso de la delegación y del nombramiento de los metodos elegidos, facilitan no solamente la facil lectura y comprensión del codigo  sino que tambien cobra mas sentido que  objeto debe responder a cada mensaje. A futuro en caso de tener un error en el código, vamos a poder encontrarlo facilmente por medio de testear paso a paso.

3) Opcion 1: 
   
   Se podría definir una sub clase cuentaCorriente o cajaDeAhorro
   
   Hace un self.class == cuentaCorriente, cuando la clase definida simplemente es CuentaBancaria.

   el metodo rojoPermitido no esta definido.
   
   la variable saldo no esta definido.


  Opción 2:
  Idem 1, se podria definir sub clase CC o CDA
  definir una variable tipo hace que dependas de tener que inicializar una variable mas, innecesario ya que definiendo una subclase y haciendo un Override del metodo extraer en la subclase ya lo solucionas. 
  falta : 
  -variables
   *tipo
   *saldo
   
  metodo rojoPermitido()
   
  Opción 3
  Esta solución va un poco mas a corde, utiliza subClases, pero no inicializa saldo de la misma cuando se hace el inherits, con lo cual se generaría un error en el       codigo.
    
  Opción 4
  Esta solución es la mas correcta, siguen sin  definirse algunas variables que se van a precisar para realizar la extraccion del monto deseado.
   
    
   #Actividad de lectura 1# 
   ¿Qué significa el acceso directo a las variables? De un ejemplo. 
   El acceso directo a las variables significa la definición de una variable dentro de un método.
   
   ejemplo:
   
   method usarPoder(unValor){
   var mana= ...
   if( mana - unValor > 0){ self.atacar()}
   }
   
   
   ¿Qué significa el acceso indirecto a las variables? De un ejemplo. 
   el acceso indirecto a las variables significa poder acceder a una variable por medio de un mensaje al objeto en cuestión. La definición se hace por fuera del metodo    y dentro del objeto.
   
   Por ejemplo:
   
   guerrero.mana()
   
   
   Qué ventajas y desventajas presenta cada estrategia referida a los getters y setters.
   
   la ventaja del directo es que aportan legibilidad al código, pero el alcance de las variables están restringidas al metodo donde estan definidas.
   otra desventaja es que una vez definidas e inicializadas las variables no se puede modificar el valor de la misma y dependen de un parametro externo para darle un      valor.
   
   la ventaja del indirecto es que por medio de mensajes se puede obtener el valor de la variable y tambien setearla. Otra ventaja es que al momendo de crear subclases solamente se definen las variables al momento de crear dicha subclase.
