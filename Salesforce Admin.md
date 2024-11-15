# Objects
Son la unidad fundamental para almacenamiento de información en salesforce. Hay 2 tipos de objetos ==Standard== (objetos predefinidos ) y ===Custom=== (Objetos creados por el usuario), los objetos custom pueden agregarse uno por uno o por medio de una hoja de datos en excel

# Relacion entre objetos
Estas relaciones permiten conectar datos entre nuestros objetos. Las más comunes son:
- Relación de busqueda (Lookup):
	Se utiliza para relacionar un objeto con otro. 
	Por ejemplo si tuvieramos un objeto "Materia" podriamos usar esta relacion para relacionar al objeto "Profesor", es decir, usariamos esta relacion para relacionar la materia a impartir con el profesor que lo hará.
- Relación Maestro-Detalle (Master-Detail):
	Se utiliza para crear una conexión de dependencia entre dos objetos (objeto detalle depende de objeto maestro). Si el objeto maestro se elimina, se elimina el objeto detalle. 
	Por ejemplo si tuvieramos un objeto llamado "Orden" (Maestro), podriamos usar esta relación con el objeto "Productos de la orden" (detalle)
# Tabs
Es la manera en que podemos organizar y acceder a los diferentes objetos creados. Cada tab es un acceso rapido a los registros de un objeto.
# Lightning App
Es una aplicacion personalizada que permiten acceder a un conjunto especifico de pestañas, objetos, herramientas y componentes organizados. Este tipo de apps son análogas a una hoja de excel, es decir, en ellas podemos guardar toda la información de nuestra empresa o donde vayamos a aplicar la app. Una vez creada la app podremos incluir los tabs y además agregar los diferentes perfiles que tendrán acceso a ella

# Fields
Son los elementos dentro de los objetos. En este caso tambien tenemos dos tipos de campos ==Standard== y ===Custom===

# Record Types
Los record types nos permiten separar en categorias a nuestros objetos, es decir, si tenemos un objeto que llamado habitación, los record types nos permiten determinar si es una habitación basica o de lujo y a su vez asiganar un page layout a cada tipo

# Validation Rules
Nos permiten determinar que los datos ingresados cumplan ciertas condiciones. Si los datos no cumplen con las reglas de validación, se muestra un mensaje de error y el registro no se guarda hasta que se corrija el error.





