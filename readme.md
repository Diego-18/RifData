# RifData
Clase java que permite obtener los datos del RIF de un contribuyente desde la p�gina del SENIAT - Venezuela

**Uso**

1. Incluir la clase Rif
2. Utilizar el m�todo `Rif.getDataRif(String NroRif)`, pasando como par�metro el nro de Rif
3. El m�todo retorna un `HashMap<String,Object>`, con un valor `String`, `Boolean` o `BigDecimal`, dependiendo de la informaci�n.
4. Si el contribuyente no existe, el m�todo `Rif.getDataRif(String NroRif)` retornar� *null*
5. Para acceder m�s f�cilmente a los datos que retorna, utilizar los keys que provee la clase:

- `Rif.NOMBRE`: el valor ser� un **String** con el nombre del contribuyente
- `Rif.NOMBRE_COMERCIAL`: el valor ser� **String** con el nombre comercial del contribuyente
- `Rif.AGENTE_RETENCION`: el valor ser� un **Boolean** que indica si el contribuyente es un agente de retenci�n o no.
- `Rif.CONTRIBUYENTE`: el valor ser� un **Boolean** que indica si el RIF proporcionado es de un contribuyente 
- `Rif.TASA`: el valor ser� un **BigDecimal** con la tasa de retenci�n del contribuyente

Ejemplo: `dataRif.get(Rif.NOMBRE)`  
