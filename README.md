# VirtualDreams
**EVALUACIÓN PRÁCTICA DE VIRTUAL DREAMS**

**EJERCICIO 2**


1.  ¿Qué es un servidor HTTP?
Cuando hablamos de servidor HTTP hablamos de hw y sw. El hw del servidor HTTTP puede ser una computora o un conjunto de las mismas las cuales tienen sw alojado. En su conjunto conforma un servidor HTTP. Los clientes acceden a dicho servidor HTTP a través de internet por medio de un dominio. Un servidor HTTP tiene URL y protocolo de navegación HTTP. 

2. ¿Qué son los verbos HTTP? Mencione los más conocidos
Los verbos HTTP son acciones que se realizan sobre un servidor y que él debe responder. O sea los verbos son acciones para realizar peticiones a un servidor. 
Los verbos HTTP mas conocidos son GET, HEAD, POST, PUT, PATCH, DELETE, TRACE, OPTIONS, CONNECT y HTTPS. Describiré los 4 verbos más usados:

GET: Me permite obtener los datos de un servidor. Para eso le paso la URL. Es una solicitud y se envía dicha solicitud cuando el cliente desea obtener información sobre un recurso del servidor.

POST: Es una solicitud que un cliente envía al servidor. Pero en este caso el cliente envía información al servidor. Una solicitud POST es similar a cuando se envía un formulario web por la red. Ya que en ese caso ud le esta enviando informacion a un servidor

DELETE: Se usa para eliminar un recurso situado en el servidor. Para lograr este objetivo necesito la URL del servidor en cuestión

PUT: Me permite crear un recurso o reemplazarlo por otro. Dicho recurso que se va a crear o reemplazar se lo envia desde el body de dicha solicitud.

3. ¿Qué es un request y un response en una cominicacion HTTP? ¿Qué son los HEADERS?
Un request es una petición que un cliente envía a un servidor. Y el response es la respuesta que devuelve el servidor al cliente. En el header va la información de control del mensaje que se desea enviar.

4. ¿Qué es un queryString? (En el contexto de una URL).
Es una cadena de consulta. Es la parte de la URL y contiene los datos q se pasan al servidor web.

5. ¿Qué es responseCode? ¿Qué signficado tiene los posbles valores devueltos?
ResponseCode son códigos de estado de HTTP Y proporciona información de estado de una solicitud. O sea son códigos que me indican si la solicitud fue o no exitosa. El signficado de los posibles valroes devuelto son:
-	Respuestas informativas en el rango 100 -199
-	Respuesta satisfacotria en el rango 200 – 299
-	Redirecciones en el rango 300 - 399
-	Errores de los clientes en el rango 400 – 499
-	Errores de los servidores en el rango 500 – 599

6. ¿Cómo se envía data en un Get y como en un POST?
Con el método get, los datos que se desean consultar desde un servidor por medio una dirección URL. 
Nomenclatura 
get www.yahoo.com.ar

El método set me permite generar datos y almacenarlos mediante a un servidor web por medio la dirección UR.
Ej del envío de datos en json mediante aplicación postman
post www.menganito.com
~~~
{
  "Name" : "Cristian",
  "Apellido" : "Famiglietti"
}
~~~

7. ¿Qué verbo http utiliza el navegador cuando accedemos a una pagina?
Usa el verbo GET ya que si usted quiere simplemente acceder a una pag web usa get. Ahora si quiere depositar información en un servidor por medio de un navegador, como ser postear algo en facebook use post.

8. Explicar brevemente que son las estructuras de datos JSON y XML dando ejemplo de estructuras posbles.
JSON es una notación de objeto de javaScript. Es un formato para el intercambio de datos con la notación de objeto de javascript. 

Ejemplo:
~~~ 
var empleado = {
	“Apellido” : “Perez”,
	“Profesion” : “Docente”
}
~~~

El objeto se llama empleado, sus atributos son apellido y profesión y sus valores respectivos son Perez y Docente.
XML es un lenguaje de marcado extensible. Se compone de etiquetas, esas etiquetas nos brinda la información que queremos procesar. Me sirve también para transportar datos legibles. Y se suele usar para representar estrucura de datos.

Ejemplo:
~~~
<empleado>
	<apellido> Perez </apellido>
	<profesión> docente </profesión>
 <empleado>
~~~

9. Explicar brevemente el estándar SOAP 
Es un protocolo que define como  pueden comunicarse entre si dos objetos por medio de intercambio XML. O sea es un formato de mensaje XML en la interacción de servicios web.

10. Explique brevemene que es REST Full
Es una API que fue diseñada bajo los conceptos de REST. Son servicios web que se basa en recursos. Estos recursos son entidades , generalmente están almacenadas en servidores y el cliente las accede.

11. ¿Qué son los headers en un request? ¿Para que se utiliza el key content-type en un header?
Los headers  request transmite información  acerca del navegador del cliente, de la pagina solicitada, del servidor, etc. 

El Content-type en un header le indica al cliente que tipo de contenido será retornado. O sea le permite a un cliente indicarle al servidor, en que formato envia los datos. Así el servidor procesa los datos sin problemas.

**EJERCICIO 3**

Recomendamos previamente entender los conceptos de la sintaxis “json” antes de arrancar con los ejercicios.
Descargar el POSTMAN (aplicación para realizar request como cliente), adjuntando un screen de resolución para cada ítem:

1.	Realizar un request GET a la URL: 
https://vdfactory-234311.firebaseio.com/contacts.json

Se documenta dicho procedimiento. Se envi el request y se visualize que arroja los siguientes datos:
~~~
{
    "-McQx4mYWSX9HBY4lekh": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxMoxrtBwlepiKQEV": {
        "email": "ignacio.nogueira@hotmail.com",
        "firstname": "Ignacio"
    },
    "-McQxQI5VIqDZ2ggzVll": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxSUGjbriHXiQ6pq-": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxUiu6PoynDI9NHGW": {
        "email": "nahuelcartasegna@gmail.com",
        "firstname": "Nahuel"
    },
    "-McQxWkPzwr_7t7v5nm2": {
        "email": "nahuelcartasegna@gmail.com",
        "firstname": "Nahuel"
    },
    "-McQxYrC_yusLW4ZL_hF": {
        "email": "mennawanda@gmail.com",
        "firstname": "Wanda"
    },
    "-McQyHnB2MnaytmfPofO": {
        "email": "mennawanda@gmail.com",
        "firstname": "Wanda"
    },
    "-McqffNZ5T7RmrXE81Kv": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McqgWJuRl_9U6lpm-MM": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MfxZULe0WLYBnjeINcv": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MfxZtXHp-Xnf3A6pOev": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-Mfx_eBY05IfJ_fyTADe": {
        "email": "Pato.Pepito@gmail.com",
        "firstname": "Pato"
    },
    "-MgLzd27XFAOJpPQvVrV": {
        "email": "juan.diaz@virtualdreams.io",
        "firstname": "Juan"
    },
    "-MgLzjG23khM6zxu-7QN": {
        "email": "melina.sanson@virtualdreams.io",
        "firstname": "Melina"
    },
    "-MjfmDab0XB9Kjp80BIa": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    }
}
~~~

Se visualizó los disntintos id que van adquiriendo las distintos usuarios. Cada id tiene atributo email y primer nombre. 

2.	Realizar un request POST a la URL anterior, y con body:

~~~
{
	"firstname":"Pablo",
	"email":"pablo.perez@virtualdreams.io"
}
~~~

Tip: (Marcar la opción “raw” como body)
Se realizó el post a la dirección en cuestión:
 
Me devolvió el ultimo id que obtuvo Pablo cuyo mail es pablo.perez@virtualdreams.io

3.	Realizar nuevamente un request GET a la URL: 
https://vdfactory-234311.firebaseio.com/contacts.json

Se documenta; arroja lo siguiente:

~~~
{
    "-McQx4mYWSX9HBY4lekh": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxMoxrtBwlepiKQEV": {
        "email": "ignacio.nogueira@hotmail.com",
        "firstname": "Ignacio"
    },
    "-McQxQI5VIqDZ2ggzVll": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxSUGjbriHXiQ6pq-": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxUiu6PoynDI9NHGW": {
        "email": "nahuelcartasegna@gmail.com",
        "firstname": "Nahuel"
    },
    "-McQxWkPzwr_7t7v5nm2": {
        "email": "nahuelcartasegna@gmail.com",
        "firstname": "Nahuel"
    },
    "-McQxYrC_yusLW4ZL_hF": {
        "email": "mennawanda@gmail.com",
        "firstname": "Wanda"
    },
    "-McQyHnB2MnaytmfPofO": {
        "email": "mennawanda@gmail.com",
        "firstname": "Wanda"
    },
    "-McqffNZ5T7RmrXE81Kv": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McqgWJuRl_9U6lpm-MM": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MfxZULe0WLYBnjeINcv": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MfxZtXHp-Xnf3A6pOev": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-Mfx_eBY05IfJ_fyTADe": {
        "email": "Pato.Pepito@gmail.com",
        "firstname": "Pato"
    },
    "-MgLzd27XFAOJpPQvVrV": {
        "email": "juan.diaz@virtualdreams.io",
        "firstname": "Juan"
    },
    "-MgLzjG23khM6zxu-7QN": {
        "email": "melina.sanson@virtualdreams.io",
        "firstname": "Melina"
    },
   "-MjfoPZP5B6AHGGcN2jU": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MjfmDab0XB9Kjp80BIa": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MjfrObrZWLCQDoIx5R4": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    }
}
~~~

¿Qué diferencias se observan entre las llamadas el punto 1 y 3?
La diferencia, es que luego de hacer el post, se le agrego un nuevo id a Pablo cuyo correo es pablo.perez@virtualdreams.io, O sea creé un nuevo registro

**EJERCICIO 4**

URL: https://trailblazer.me/id/cfamiglietti2

**EJERCICIO 5**

LEAD: Representa un cliente potencial de venta. Es cun cliente potencial para mi producto o para mi empresa. Los datos que almacena de forma estándar son

ACCOUNT: Representa un consumidor, una empresa, cliente socio, competidor al cual se le realiza algún tipo  de seguimiento. Los datos que almacena de forma estándar son CONTACT: Es una persona que se encuentra vinculada con su propia cuenta. 

Opportunity: Representa una oportunidad de venta o una oportunidad de un trato pendiente. 
Product: Representa los servicios y artículos que vende una empresa. 

PriceBook: Representa una lista de precios que tiene una lista de productos que vende una empresa.

Quote: Registra los precios propuestos para los distintos servicios y productos. 

Asset: Es un tipo de producto que posee un cliente. Pueden ser os productos de la competencia como de mi empresa. 

CASE: Representa una descripción de los comentarios, problemas o preguntas que realiza un cliente. De esta manera uno puede rastrear y resolver los problemas e inquietudes que tiene un cliente. 

Article: Representa la información sobre servicios y productos de una empresa que desea que este disponible en su base de conocimientos. 
 
	 
Los datos que almacena lead de forma estándar son:
1. Address		
2. Annual Revenue		
3. Campaing
4. Clean Status		
5. Company			
6. Company D-U-N-S Number
7. Created By		
8. Current Genrator(s)		
9. D&B Company
10. Data.com Key		
11. Description			
12. Do Not Call
13. Email		
14. Email Opt Out		
15. Fax
16. Fax Opt Out		
17. Individual			
18. Industry
19. Las Modified By	
20. Last Transfer Data		
21. Lead Owner
22. Lead Source		
23. Lead Status			
24. Mobile
25. Name			
26. No. Of Employees		
27. Number of Locations
28. Phone		
29. Primary			
30. Product Interest
31. Rating		
32 SIC Code			
33 Title
34. Website		

Los datos que almacena account de forma estándar son:
1. Account Name			
2. Account Number	
3. Account Owner
4. Account Site 		
5. Account Source	
6. Active
7. Annual Revenue		
8. Billing Address	
9. Clean Status
10. Created By			
11. Customer Priority	
12. D&B Company
13. Data.com Key		
14. Description		
15. D-U-N-S Number
16. Employees			
17. Fax			
18. Industry
19. Last Modified By		
20. NAICS Code		
21. NAICS Description
22. Number of Locations		
23. Owership		
24. Parent Account
25. Phone			
26. Rating		
27. Shipping Address
28. SIC Code			
29. SIC Description	
30. SLA
31. SLA Expiration Data		
32. SLA Serial Number 	
33. Ticker Symbol
34. Tradestyle			
35. Type			
36. Upsell Opportunity
37. Website		

Los datos que almacena contact de forma estándar son:
1. Account Name			
2. Assistant				
3. Asst. Phone
4. Birthdate			
5. Clean Status				
6. Contact Owner
7. Created By			
8. Data.com Key				
9. Department
10. Description			
11. Do Not Call				
12. Email
13. Email Opt. Out		
14. Fax					
15. Fax Opt. Out
16. Home Phone			
17. Individual				
18. Languages
19. Last Modified By		
20. Last Stay-in-touch Request Data	
21. Last Stay-in-touch Save Data
22. Lead Source			
23. Level				
24. Loan Amount
25. Location			
26. Mailing Address			
27. Mobile
28. Name				
29. Other Address			
30. Other Phone
31. Phone			
32. Reports To				
33. Title
		

Los datos que almacena opportunity de forma estándar son:
1. Account Name				
2. Amount 			
3. Close Date
4. Contract				
5. Created By			
6 Current Generator(s)
7. Delivery/Instalation Status		
8 Description			
9. Expected Revenue
10. Forecast Category			
11. Last Modified By		
12. Lead Source
13. Main Competition(s)			
14. Next Step			
15. Opportunity Name
16. Opportunity Owner			
17. Opportunity Score		
18. Order Number
19. Price Book				
20. Primary Campaign Source	
21. Private
22. Probability(%)			
23. Quantity			
24. Stage
25. Tracking Number			
26. Type	
		

Los datos que almacena product de forma estándar son:
1. Active			
2 Created By			
3. Display URL
4. External Data Source		
5. External ID			
6. Last Modified By
7. Product Code			
8. Product Description		
9. Product Family
10. Product Name			
11. Product SKU			
12. Quantity Unit Of Measure

Los datos que almacena Price book de forma estándar son:
1. Active			
2. Created By		
3. Description
4. Is Standard Price Book	
5. Last Modified By	
6. Price Book Name

Los datos que almacena asset de forma estándar son:
1. Account			
2. Asset Level				
3. Asset Name
4. Asset Owner			
5. Asset Provided By	 		
6. Asset Serviced By
7. Competitor Asset		
8. Contact				
9. Created By
10. Current Amount		
11. Current Lifecycle End Date		
12. Current Monthly Recurring Revenue
13. Current Quantity		
14. Description				
15. Digital Asset Status
16. External ID			
17. Has Lifecycle Management		
18. Install Date
19. Internal Asset		
20. Last Modified By			
21. Lifecycle End Date
22. Lifecycle Start Date		
23. Manufacture Date			
24. Parent Asset
25. Price			
26. Product				
27. Product Code
28. Product Description		
29. Product Family			
30. Product SKU
31. Purchase Date		
32. Quantity				
33. Root Asset
34. Serial Number		
35. Status				
36. Status Reason
37. Total lifecycle  Amount	
38.  Unique Identifier			
39. Usage End Date

Los datos que almacena case de forma estándar son:
1. Account Name			
2. Asset					
3. Business Hours
4. Case Number			
5. Case Origin				
6. Case Owner
7. Case Reason			
8. Closed When Created			
9. Contact Email
10. Contact Fax			
11. Contact Mobile			
12. Contact Name
13. Contact Phone		
14. Created By				
15. Date/Time Closed
16. Date/Time Opened		
17. Description				
18. Engineering Req Number
19. Entitlement Name		
20. Entitlement Process End Time		
21. Entitlement Process Start Time
22. Escalated			
23. Internal Comments			
24. Last Modified By
25. Milestone Status		
26. Milestone Status Icon		
27. Parent Case
28. Potential Liability		
29. Priority	 			
30. Product
31. Product			
32. Service Contract			
33. SLA Violation
34. Status			
35. Stopped				
36. Stopped Since
37. Subject			
38. Type					
39. Web Company
40. Web Mail			
41. Web Name				
42. Web Phone

	 
Adjunto la relacipon entre objetos en el siguiente link publico de drive:
	
[LINK DEL DIAGRAMA](https://drive.google.com/drive/folders/1HDl9Xb3PPREFSpteQ9XBNdyq2mbVqcxA)
	
	 
**EJERCICIO 6**

A.	Consultar tu ID haciendo un GET con POSTMAN a este WS:
https://vdfactory-234311.firebaseio.com/contacts.json

Documento el procedimiento:
 
Los id arrojados son

~~~
{
    "-McQx4mYWSX9HBY4lekh": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxMoxrtBwlepiKQEV": {
        "email": "ignacio.nogueira@hotmail.com",
        "firstname": "Ignacio"
    },
    "-McQxQI5VIqDZ2ggzVll": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxSUGjbriHXiQ6pq-": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McQxUiu6PoynDI9NHGW": {
        "email": "nahuelcartasegna@gmail.com",
        "firstname": "Nahuel"
    },
    "-McQxWkPzwr_7t7v5nm2": {
        "email": "nahuelcartasegna@gmail.com",
        "firstname": "Nahuel"
    },
    "-McQxYrC_yusLW4ZL_hF": {
        "email": "mennawanda@gmail.com",
        "firstname": "Wanda"
    },
    "-McQyHnB2MnaytmfPofO": {
        "email": "mennawanda@gmail.com",
        "firstname": "Wanda"
    },
    "-McqffNZ5T7RmrXE81Kv": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-McqgWJuRl_9U6lpm-MM": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MfxZULe0WLYBnjeINcv": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MfxZtXHp-Xnf3A6pOev": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-Mfx_eBY05IfJ_fyTADe": {
        "email": "Pato.Pepito@gmail.com",
        "firstname": "Pato"
    },
    "-MgLzd27XFAOJpPQvVrV": {
        "email": "juan.diaz@virtualdreams.io",
        "firstname": "Juan"
    },
    "-MgLzjG23khM6zxu-7QN": {
        "email": "melina.sanson@virtualdreams.io",
        "firstname": "Melina"
    },
    "-MjfmDab0XB9Kjp80BIa": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MjfoPZP5B6AHGGcN2jU": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-MjfrObrZWLCQDoIx5R4": {
        "email": "pablo.perez@virtualdreams.io",
        "firstname": "Pablo"
    },
    "-Mjl-TMa7Sn1YHsjAppH": {
        "email": "cristian.famiglietti@virtualdreams.io"
    }

}
~~~

Mi mail es cristian.famiglietti@virtualdreams.io- Es el último registro que se visualiza en formato Json en el código presentado arriba. El mismo es el siguiente

~~~
 "-Mjl-TMa7Sn1YHsjAppH": {
        "email": "cristian.famiglietti@virtualdreams.io"
    }
~~~

Como se visualiza, mi id es Mjl-TMa7Sn1YHsjAppH

Parte C del ejercicio:

~~~
trigger TriggerEjercicio6_c on Contact (before insert, before update) {   
    for(Contact co: Trigger.New){
        if(co.idvirtualdreams__c=='-Mjl-TMa7Sn1YHsjAppH'){
            system.debug(co.Name + ' - ' + co.Email);     
            co.Email = 'cristian.famiglietti@virtualdreams.io';
                      
        }
    }    
}
~~~


**EJERCICIO 7**

SOLUCIONES DE SALESFORCE

A.	¿Qué es Salesforce?
Salesforce  es una compañía PaaS (Plataforma como Servicio) para desarrollar aplicaciones desde internet.  Es una plataforma que facilita la relación comerciales con los clientes (Conocido como CRM), mateniendo un contacto contínuo con los mismos. Produce un CRM llamado Sales Cloud. O sea basa su plataforma en la nube para que ventas, marketing, comercio electrónico y servicio al cliente puedan tener una visión unificada del cliente usando tecnología B2B (de empresa a empresa)  y B2C (de la empresa al consumidor final)

B.	¿Qué es Sales Cloud?
Es una plataforma de venta que otorga seguimiento al proceso de ventas, desde perfilar leads,  hacer el contacto inicial  hasta el final de la compra. Ofrece productos Salesforce en la nube. O sea hace referencia a las ventas mediante la nube. Permite gestionar de manera eficiente los clientes, la colaboración entre equipos comerciales, optimizando los procesos comerciales alineándose con el marketing y servicio de atención al cliente.

C.	¿Qué es Service Cloud?
Es servicio en la nube que ayuda a las empresas y a sus clients, atendiendo las necesidades de informacion de los clientes.

D.	¿Qué es Health Cloud?
Es una plataforma que permite gestionar la relación medico-paciente. Unifica toda la informacion en una misma plataforma y procedente de distintas Fuentes.  Los pacientes pueden hacer uso de esta plataforma en cualquier momento y desde cualquier dispositivo, pudiendo contactar e interactuar fácilmente con el personal medico. O sea es una plataforma destinada  para la gestión de pacientes por medio de la nube, lo cual ofrece comunicación eficaz entre pacientes, personal médico,  y demás. Esta plataforma hace un uso eficiente de los datos medios, servicios y procesos clínicos, adaptándose al perfil de cada paciente. 


E.	¿Qué es Marketing Cloud?
Es una plataforma en la nube para lograr una mayor cercanía  de la marca de un producto con el cliente. Está dirigido al equipo de marketing, así el mismo puede mejorar su experiencia con los clientes y aumentar las ventas de la empresa. Contiene herramientas para gestionar de manera eficiente los clientes y potenciales clientes, a través de distintos canales. 

FUNCIONALIDADES DE SALESFORCE

A.	¿Qué es un RecordType?
Me ayuda a mostrar registros a los usuarios por medio de Pages Layouts, Business process  y demás. Entre ellos, la info que muestra dichos registros son distitna información según el perfil del usuario. Tambien me permiten obtener diferentes procesos comerciales,  diseños de página en distintos formatos. Puede crear RecordType para diferenciar sus acuerdos de ventas habituales de sus compromisos de servicios profesionales, ofreciendo diferentes valores de lista de selección para cada uno. 

B.	¿Qué es un ReportType?
Son tipos de informes. Según el tipo de informe que genere, voy a tener distintos campos en mis registros. Por ejemplo puedo agarrar los objetos tipo Cuenta y generarle un checkbox para que tilde las casas que ya fueron vendidas

C.	¿Qué es un Page Layout?
Son diseños de pagina que me permiten tener un control de botones, lables, visualforce y demás elementos. Tambien me permite decidir que campos son visibles y cuales no.


D.	¿Qué es un Compact Layout?
Me permite visualizar aspectos importantes en el encabezado de una página. Para cada objeto se puede asignar como mucho diez campos, incluyendo el campo nombre. 

E.	¿Qué es un Perfil?
Los perfiles definen a qué datos y objetos tiene permitido hacer un usuario con cierto rol en la aplicación

F.	¿Qué es un Rol?
El rol es la responsabilidad que se le asigna a un usuario,cuenta de socio o contacto para cuentas y oportunidades. Los administradores pueden configurar el rol de los usuarios. Los usuarios individuales puden asignar roles específicos a socios y contactos.

G.	¿Qué es un Validation Rule?
Una regla de validación evita que se guarden registros que no cumplan con los estándares definidos. O sea las vaidation rules verifican que el usuario ingrese registros según ciertos estándares predefinidos. Un ejemplo puede ser una fórmula que evalúa los datos en algunos campos ofreciendo  un valor  true o false. Si la regla de validación devuelve true significa que los datos ingresados por el usuario contiene algún valor  inválidos, caso contrario significa que los campos son válidos. Por medio de las validation rules se puede mejorar la calidad de los datos.  	

H.	¿Qué diferencia hay entre una relación Master Detail y Lookup?
Lookup son relaciones de búsqueda. Una relación de búsquda vincula dos objetos.  Consiste en buscar un objeto en los elementos relacionados del otro objeto. Sin embargo la relación Master Detail también conocida como relación principal-detalle un objeto toma el papel de principal y  el otro objeto es el objeto detalle. El objeto principal, como su nombre lo indica, controla ciertos comportamientos del objeto detalle.

I.	¿Qué es un Sandbox?
Es una copia casi exacta de una organización para desarrollo, pruebas y capacitación. 
Los entornos sandbox estan aislados de la organización, asi las operaciones que se realizan no le afecta  a la organización en sí. Tenemos varios tipos de sandbox como ser	sandbox de desarrollo, sandboox Developor Pro,  sandbox de copia parcial y sandbox completo. 

J.	¿Qué es un ChangeSet?
Me permite hacer cambios personalizados, como ser crear nuevos objetos. Esto se ve reflejado en cambios en la organización. Los ChangeSet hacen referencia a cambios a nivel información de la empresa desde salesforce.

K.	¿Para qué sirve el import Wizard de Salesforce?
Es un asistente para importar datos de manera eficiente en Salesforce. Esto lo realiza un adminstrador: agrega y actualiza los registros cuando accede a nuevos datos.  Permite importar datos como ser cuentas contactos, clientes, soluciones, etc. Puede importar hasta 50 mil registros a la vez. 

L.	¿Para qué sirve la funcionalidad Web to Lead?
Es una hta de marketing pa atraer nuevos visitantes a un sitio web y asi convertirlos en futuros clientes.  Para eso se le pide al visitante que llene un formulario dentro del sitio web donde ingresan info sobre productos de interés y demás. Y de esta manera se busca q el visitante se convierta en un potencial cliente. Los leads son clientes potenciales. Se los considera como tal ya que demuestran cierto interés en nuestro producto y servicio. Por ende son una oportunidad de negocio para la empresa. Se busca convertir estos clientes potenciales en clientes mediante estrategias de marketing. 

M.	¿Para qué sirve la funcionalidad Web to Case?
Un case es una inquietud, problema, comentario o pregunta que tiene un cliente. Los operadores analizan estos casos y buscan solucionar el problema e inconveniente que puede tener el cliente. 

N.	¿Para qué sirve la funcionalidad Omnichannel?
Permite q un cliente se  conecte con un personal de soporte por medio de multiples canales. A la vez, el personal de soporte tienen acceso inmediato al cliente al que está a punto de ayudar. Le permite a los agentes, recibir casos (cases)por medio de  la plataforma a través de distintos canales ya sea por medio de email, chat, etc canales distintos. Todo esto se logra con esta herramienta.


O.	¿Para qué sirve la funcionalidad Chatter?
Es una app que permite que los usuarios trabajen colaborativamente, para que ellos puedan también comunicarse y compartir información.  Permite colaborar entre usuarios por ejemplo en oportunidades de ventas, casos de servicio, proyectos, campañas, etc. 

CONCEPTOS GENERALES:

A.	¿Qué significa SaaS? 
El sw como servicio permite q los usuarios se conecten y usen aplicaciones que estan la nube mediante algún dispositivo conectado a internet. Ejemplo de SaaS son  el email , Word de google, etc.

B.	¿Salesforce es Saas?
Salesforce es PaaS (Plataforma como Servicio) y  SaaS(sw como servicio) ya que en dicha plataforma se ofrece varios servicios al cliente y a las empresas

C.	¿Qué significa que una solución sea Cloud?
Antiguamente tenias la aplicación archivos, fotos y documentos en tu propia máquina. Si no tenias la maquina contigo no podias acceder a los mismos, salvo que te los lleves en un dispositivo externo. Ahora no hace falta un dispositivo externo, al tenerlo en la nube, podes acceder a tus documentos, archivos, fotos, aplicaciones desde la nube. De hecho podes manipular archivos con aplicaciones que vienen incluida en la nube.

D.	¿Qué significa que una solución sea On-Premise?
Es distinto al sw en la nube, ya que  el sw se instala tanto en los servidores como en equipoa locales de la empresa. La ventaja es que la empresa se encarga del control fisico  de la configuracion del sistema ademas de la seguridad

E.	¿Que es un pipeline de ventas?
Es un conjunto de actividades diarias q componen una venta en cada etapas de una negociacion. O sea son las distintas fases por las cuales pasa una venta

F.	¿Que es un funnel de ventas?
Es la forma en que una empresa piensa, planea y crea procesos para atraer personas desconocidas  y convertirlas en clientes.

G.	¿Qué significa Customer Experience?
Es una estrategia de marketing (de hecho hay empresas q tienen un departamento exclusivo de customer experience). El customer experience es el punto de contacto que tiene la empresa que ofrece el producto/servicio con el cliente. Y este punto de contacto le genera valor a la empresa, ya que conoce las expectativas que tiene el cliente con la marca, le permite ver a la empresa donde estan parado con respecto a ellos mismos como con respecto a sus competidores. 

H.	¿Qué significa omnicanalidad?
Es una estrategia de comunicación para que la empresa esté en contacto con el cliente por medio de varios canales como ser mail, telefoncimanete, mensaje de texto, cara a cara, etc

I.	¿Qué significa que un negocio sea B2B?
Business to business (B2B) se refiere a la comunicación e interaccion comercial entre dos empresas. O sea es una estrategia de marketing donde el ojetivo es la interaccion entre compañias y se deja de lado el consumidor final. 

J.	¿Qué significa que un negocio sea B2C?
Signfica del negocio al consumidor, o sea se refiere a la actividad comercial entre la empresa y el consumidor final

K.	¿Qué es un KPI?
Son indicadores clave de rendimiento. Se los usa para evaluar el éxito que se tiene al aplicar ciertas acciones, ciertos procesos. Mientras mejores sean los indcadores claves de rendimiento significa que mas alineado estoy con la concrecion de mis objetivos. Se los usa en varios contexto, si lo vemos a nivel empresa tenemos indicadores claves de rendimiento en area de marketing, financiero, comercial, area de calidad, etc. 

L.	¿Qué es una API y en qué se diferencia de una Rest API?
Una API (interfaz  de programacion de aplicacione) Permite q aplicaciones se comuniquen entre si, sin necesidad de saber coo estan implementadas, a traves de un conjunto de reglas.  

La diferencia con REST API es que  este ultimo permite interaccion con servicios web


M.	¿Qué es un Proceso Batch?
El proceso batch o proceso por lotes es un proceso en el cual la computadora recibe un lote de trabajos de gran volumen y los ejecuta secuencialmente, sin necesidad de interactuar con el usuario. 

N.	¿Qué es Kanban?
Es una metodologia agil. Tienen un control de tareas realizadas y a realizar por cada iteracion mediante un tablero visual de tareas. Dicho tablero es accedido por todos los miembros del equipo. El tablero mas basico tiene 3 columnas: tareas por hacer, tareeas en proceso y tareas hechas. Me permite detectar donde hay cuellos de botella para tomar decisiones para reducir los mismos. 

O.	¿Qué es un ERP? 
ERP (planificacion de recursos empresariales) hace referencia al sw que usa las empresas para gestionar las actividades de la organización ya sea gestion de riesgos, gestion de proyectos, finanzas, contaduría, etc. 

P.	¿Salesforce es un ERP?
Salesforce es un ERP ya q si bien esta centrado en el clienre(CRM), tmb gestiona sus recursos empresariales, planfica su comercializacion y su gestion con los clientes.

Una vez finalizada la práctica enviar solo el link del repositorio a ariel.tarsitano@virtualdreams.io
