# RifData
Clase java que permite obtener los datos del RIF de un contribuyente desde la p�gina del SENIAT - Venezuela

**Uso**

1. Incluir la clase `RifDataConnection`
2. Utilizar el m�todo `RifDataConnection.getDataRif(String NroRif)`, pasando como par�metro el nro de Rif
3. El m�todo retorna un objeto `Rif` con los datos del rif.
4. Si el contribuyente no existe, el m�todo `RifDataConnection.getDataRif(String NroRif)` generar� la excepci�n `RifNoExisteException`
5. Para acceder m�s f�cilmente a los datos que retorna, utilizar los m�todos de la clase RIF
Ejemplo: `rifdata.getNombre()`  

**Ejemplo**



	Rif rifdata = RifDataConnection.getDataRif(rif);
	System.out.println(rifdata);
	System.out.println(rifdata.getNombre());


