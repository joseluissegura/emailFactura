# emailFactura
email factura electronica

envia correo con los 3 documento factura.xml, xml-response y pdf al cliente

Ej en php:

* emailFactura("50621021800112610049300100001010000011681100011681");

----------------------------------------------
para configurar el servidor de correos crear un archivo.ini con los siguientes datos

* [email]
*   host = smtp.gmail.com
*   username = xxxxxxxxx@gmail.com
*   password = ppppppp
*   from =  xxxxxx@gmail.com
*   from_url = 'xxxxxxx.com'
----------------------------------------------

la configuracion de los directorios de templates,facturas y configuracion del email esta en: config.ini

* [dirs]
*   template_dir = ./template/
*   facturas_dir = ./Facturas/
*   email_dir = ../emailconfig/email_config.ini

----------------------------------------------

las dependecias de este proyecto estan en composer

----------------------------------------------

se recomienda aumentar el uso de memoria en php.ini para la creacion del pdf
memory_limit = 256M
