# P2_Simontacchi
<h1 align='center'>
<b>Informe Telecomunicaciones</b>
</h1>

![Portada](https://bit.coit.es/wp-content/uploads/2020/07/formando-ingenieros-de-telecomunicacion-imagen.png)

### Contexto:
Este es el segundo proyecto individual de la carrera de Ciencia de Datos de Henry. En el simulo ser contratado como analista de datos por una empresa de telecomunicaciones que quiere emmpezar a invertir en Argentina. 

## Elección de los datos: 
Para el presente trabajo se tiene el siguiente dataset obtenido de la página del ENACOM (https://indicadores.enacom.gob.ar/datos-abiertos-servicios )  
### Nombre de la Tabla: descripción del contenido
**_Internet_**: Esta tabla contiene en total 15 hojas en donde se detalla datos correspondientes a la conexión de internet correspondiente a la Republica Argentina desglosado por provincia o por localidad, por trimestre desde el 2014 hasta el 2024. En las diferentes hojas se puede tener el total de hogares, población, porcentajes, penetración discriminados por velocidad de conexión, tipo de tecnología (ADSL, Cablemodem, Fibra óptica, Wireless, Otros) e ingresos </br >

**_Telefonía Móvil_**: información sobre la cantidad de llamadas, minutos totales, acceso y penetración. Discriminados por prepago y pospago y trimestre desde el año 2013. También cuenta con una hoja de ganancias por trimestre y de casos de problemas, aunque está hoja no se encuentra muy detallada.     </br >

**_Televisión_**: Se brinda la información del acceso y penetración de la TV descrinado por paga y aire. También por provincia y por trimestre desde el año 2014. </br >

**_Telefonía Fija_**: Datos de la totalidad de telefonía fija, el acceso por hogares, comercial, gobierno, otros. También la penetración y el acceso cada 100 habitantes y 100 hogares y la ganancia total. Todos los datos por provincia y trimestre desde el año 2014.  
**_Portabilidad_**: Se brinda la portabilidad total por mes para la República Argentina desde el año 2012 hasta el 2024. </br >

**_Servicios Postales_**: Información sobre el total de ventas y unidades tanto postales como telegráficas y monetarias. Desglosado por trimestre, por mes y por provincia. También se cuenta con el personal empleado por trimestre. Desde el año 2013 hasta el 2025. </br >

**_Mapa Conectividad_**: Esta tabla contiene la disponibilidad de tecnología (ADSL, Cablemódem, Dial Up, Fibra óptica, Satelital, Wireless, Telefonía Fija, 3G, 4G) por Localidad. Para tener en cuenta la división política de Argentina es Provincias → Partidos → Localidades, por lo que la información que se brinda es el nombre de la Localidad, a que Partido pertenece y en que Provincia se encuentra. También se da información de la población.  </br >

La principal fuente del presente análisis proviene de la tabla “Internet” debido a que es la principal actividad de la empresa. De esta se eligió las hojas donde se detallan los datos a nivel provincial y totales. De esta manera se deja de lado el desglose por partidos y localidades dejando la posibilidad de hacer un análisis con mayor detalle si el cliente así lo requiere. Este criterio se tendrá en cuenta para todas las tablas, salvo para “Mapa Conectividad” donde se tomará el dato de la población para determinar los potenciales clientes, sin embargo, se hará una transformación de los datos de manera tal que me de los datos por provincia y no por localidad. La tabla “portabilidad” se utilizará completa, ya que cuenta con solo una hoja donde se muestra la portabilidad total por trimestre. 
De la tabla Televisión, se utilizará los datos de acceso totales por año, trimestre y tipo de televisión (satelital y por suscripción) 
La tabla de telefonía fija solo se utilizará la hoja de accesos totales, discriminada por Total, Hogares, Comercio, Gobierno y otros.

### Estructura
- `Dataset/`: Carpeta que ontiene las planillas excell con los datos utilizados para realizar el análisis.
- `notebooks/`: Jupyter notebooks. Dentro de esta carpeta encontraran dos archivos jupyter notebook </br >
              EDA.ipynb: Aquí se realiza el proceso de extracción, transformación de los datos. Se identificaron y eliminaron datos redundantes, atípicos y nulos, preparando la información para un análisis más limpio y efectivo para el análisis exploratorio de datos con el objetivo de identificar tendencias, distribuciones y valores críticos. Las conclusiones de este análisis se utilizaron para diseñar el dashboard y se presentan en el archivo "Informe_EDA_Telecomunicaciones.pdf".
- `Informe_EDA_Telecomunicaciones.pdf`: Informe detallado del análisis de los datos con conclusiones.
- `README.md`: El archivo que estás leyendo.

### Autor:
Laucha Logico - Contacto: [LinkedIn](www.linkedin.com/in/lautaro-simontacchi-75b77580). [Instagram](https://www.instagram.com/laucha_logico/)
