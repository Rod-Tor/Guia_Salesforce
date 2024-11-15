# Objects
Son la unidad fundamental para almacenamiento de información en salesforce. Hay 2 tipos de objetos ==Standard== (objetos predefinidos ) y ==Custom== (Objetos creados por el usuario), los objetos custom pueden agregarse uno por uno o por medio de una hoja de datos en excel

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

| **Tipo de Campo**                                                 | **Descripción**                                                                     | **Ejemplo de Uso**                                          |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| **Text (Texto)**                                                  | Almacena cadenas de texto.                                                          | Nombre del cliente, Dirección de correo electrónico         |
| **Text Area (Área de Texto)**                                     | Almacena párrafos cortos de texto.                                                  | Notas adicionales, Descripción corta                        |
| **Long Text Area (Área de Texto Larga)**                          | Almacena texto extenso de hasta 32,768 caracteres.                                  | Descripción detallada del caso                              |
| **Rich Text Area (Área de Texto Enriquecido)**                    | Almacena texto con formato HTML.                                                    | Descripción con formato, incluyendo negritas o enlaces      |
| **Number (Número)**                                               | Almacena valores numéricos enteros o decimales.                                     | Edad, Cantidad de productos                                 |
| **Currency (Divisa)**                                             | Almacena valores monetarios.                                                        | Precio del producto, Valor de la oportunidad                |
| **Percent (Porcentaje)**                                          | Almacena valores porcentuales.                                                      | Porcentaje de avance en una oportunidad                     |
| **Date (Fecha)**                                                  | Almacena solo fechas sin horas.                                                     | Fecha de nacimiento, Fecha de creación                      |
| **Date/Time (Fecha/Hora)**                                        | Almacena fechas con horas.                                                          | Fecha y hora de cierre, Fecha y hora de última modificación |
| **Checkbox (Casilla de verificación)**                            | Almacena valores booleanos (sí/no).                                                 | ¿Activo?, ¿Cliente potencial calificado?                    |
| **Picklist (Lista desplegable)**                                  | Muestra una lista de opciones predefinidas para selección.                          | Estado de la oportunidad: "Prospecto", "Cerrado - Ganado"   |
| **Multi-Select Picklist (Lista de selección múltiple)**           | Permite seleccionar múltiples opciones de una lista.                                | Habilidades del candidato, Preferencias del cliente         |
| **Lookup Relationship (Relación de búsqueda)**                    | Relaciona un registro con otro de un objeto distinto.                               | Contacto asociado con una Cuenta                            |
| **Master-Detail Relationship (Relación Maestro-Detalle)**         | Relaciona registros en una estructura jerárquica con dependencia entre objetos.     | Registro de línea de pedido vinculado a un pedido           |
| **Formula (Fórmula)**                                             | Calcula un valor automáticamente en base a otros campos del registro.               | Precio total calculado como Cantidad * Precio Unitario      |
| **Roll-Up Summary (Resumen acumulado)**                           | Muestra datos agregados (como suma, promedio) de registros de detalle relacionados. | Suma de todos los valores de pedidos para una cuenta        |
| **Auto Number (Número Automático)**                               | Genera un número único automáticamente para cada registro.                          | ID del cliente, ID de la factura                            |
| **Geolocation (Geolocalización)**                                 | Almacena coordenadas geográficas (latitud y longitud).                              | Ubicación de la dirección del cliente                       |
| **Email**                                                         | Almacena direcciones de correo electrónico.                                         | Correo electrónico de contacto                              |
| **Phone (Teléfono)**                                              | Almacena números de teléfono.                                                       | Teléfono del cliente, Teléfono de contacto                  |
| **URL**                                                           | Almacena enlaces de sitios web.                                                     | Sitio web del cliente, Perfil en redes sociales             |
| **Encrypted Text (Texto Encriptado)**                             | Almacena texto cifrado para información confidencial.                               | Número de tarjeta de crédito, Número de seguro social       |
| **Time (Hora)**                                                   | Almacena una hora específica sin fecha.                                             | Hora de apertura, Hora de cierre                            |
| **External Lookup Relationship (Relación de búsqueda externa)**   | Relaciona un registro con un registro externo en otro sistema.                      | Identificación de cliente en un sistema externo             |
| **Indirect Lookup Relationship (Relación de búsqueda indirecta)** | Conecta un objeto externo a un objeto estándar de Salesforce.                       | Conexión entre un objeto externo y una cuenta en Salesforce |

# Record Types
Los record types nos permiten separar en categorias a nuestros objetos, es decir, si tenemos un objeto que llamado habitación, los record types nos permiten determinar si es una habitación basica o de lujo y a su vez asiganar un page layout a cada tipo. Los record types nos permiten personalizar la forma en que se muestra y gestiona la información dentro de un mismo objeto, de esta forma dentro de un mismo objeto podemos usar diferentes:
- Procesos de negocio
- Layouts
- Opciones de picklist

# Validation Rules
Nos permiten determinar que los datos ingresados cumplan ciertas condiciones. Si los datos no cumplen con las reglas de validación, se muestra un mensaje de error y el registro no se guarda hasta que se corrija el error.





