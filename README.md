# ERA5_Tiputini
Automatic script to download, store and create graphics for tiputini station located at the amazonia region of Ecuador

Protocolo de descargas y actualización datos climáticos – Estación Tiputini

Consultor: Manuel Narváez 

1.	Descarga e instalación de programas y software necesarios

Se puede utilizar los scripts llamados setup.bat (Windows) o setup.sh (Mac o Linux) para instalar Python, jupyter y las librerías necesarias. 
-	Para Windows: Abrir Command Prompt, Navegar hasta el Directorio donde está setup.bat y Correr el código escribiendo setup.bat 
-	Para Mac o Linux: Abrir una Terminal,  Navegar hasta el directorio donde está setup.sh, colocar chmod+x setup.sh en el terminal y Correr el script mediante ./setup.sh 

Si los scripts no funcionan se lo puede realizar por medio de los siguientes pasos:
-	Descargar anaconda desde el siguiente url: https://www.anaconda.com/ 
-	Seguir los pasos recomendados para la instalación
-	Una vez instalado anaconda se debe descargar e instalar las librerías necesarias:
o	tkinter 
o	netCDF4
o	numpy 
o	xarray 
o	dask 
o	geopandas 
o	matplotlib 
o	contextily 
o	rasterstats 
o	era5cli 
El proceso se indica en los siguientes pasos
1.	Abrir Anaconda
 
2.	Instalar Jupyter Notebook o Jupyter Lab (Aparecerá in verde la palabra install)
  
3.	Entrar a Environments 
 
4.	En environments crear un nuevo environment (cualquier nombre) con Python 3.11.9
 
5.	Instalar las librerías necesarias (Seleccionar All, escribir el nombre de la librería eg: tkinter, dar click al checkbox, se abrirá una ventana en donde dirá instalar)
 
6.	Realizar este paso para todas las librerías mencionadas, si anaconda no encuentra la librería a instalar se puede realizar el siguiente proceso:
a.	Abrir Qt Console 
 
b.	Y escribir en la terminal Qt pip install ´nombre de la librería´eg tkinter
 

7.	Finalmente abrir Jupyter Notebook o Jupyter Lab
 

Antes de empezar a utilizar el código para la descarga de datos desde Copernicus (Datos  Satelitales y de reanálisis ERA5) se debe configurar usuario y key para empezar la descarga:
1.	Se debe utilizar el usuario y clave disponible por la estación Tiputini o generar uno nuevo en la siguiente pagina https://cds.climate.copernicus.eu/#!/home
2.	Una vez creado o abierto el usuario se debe ir al perfil del usuario y copiar los números de UID y API Key (Para el ejemplo utilizaremos los datos del consultor pero se pide que la estación disponga de un usuario propio y contraseña)
 

3.	Estos datos se deben copiar en un terminal “Command Promp” (o cualquier terminal en el caso de Mac o Linux) de la siguiente manera era5cli config --uid ID_NUMBER --key "KEY"
 
4.	La terminal regresara el texto Keys succesfully validated and stored in ….. si el proceso se realizó bien.

Una vez instalado todo, al abrir Jupyter Noptebook o Jupyter Lab desde anaconda o directamente, se abrirá una ventana en Chrome, Mozilla o Edge, dependiendo de cual sea el buscador de la laptop. Dentro de esta ventada se debe buscar el documento entregado por el consultor llamado Protocolo.ipynb

 

Para empezar a realizar las descargas y actualizaciones se deben seguir las instrucciones del script.


