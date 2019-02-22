# Hx711
Programa .ino para manejo de galga hx711, tener en cuenta que se debe descargar la libreria adicional para que funcione. https://github.com/bogde/HX711 (actualizada a febrero de 2019) 
Contiene diagrama de conexion 
SI usan la libreria de bodge deben realizar el siguiente cambio al codigo:
//////////////////////////////////////////////////////////
HX711 scale(5, 6);
Reemplazarlo por:

/////////////////////////////////////////////////////////
const int LOADCELL_DOUT_PIN = 5;
const int LOADCELL_SCK_PIN = 6;

HX711 scale;
//////////////////////////////////////////////////////////
De lo contrario pueden usar la libreria en el .rar de este git
