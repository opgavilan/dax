# Documentación
## HASONEVALUE
### Escenario 1. HASONEVALUE+SEGMENTACIÓN DE DATOS
Para este escenario el HASONEVALUE, es aplicado con la segmentación de datos, ya que esta haciendo referencia a la columna [Tipo Escenario] de la tabla parametros, donde si es único, podremos aplicar la siguiente operación. Los valores de [porcentaje.decimal], ayudan en dar un proyectado sobre la medida [VentaTotal].

```
=IF(HASONEVALUE(parametros[Tipo Escenario]); //Si tiene un solo valor es TRUE    
	[VentaTotal] * (1+VALUES(parametros[porcentaje.decimal]));  //Operación en caso sea TRUE      
	BLANK()    
 )
```
[01.HasoneValue_KPIS.xlsx](https://github.com/user-attachments/files/16302996/01.HasoneValue_KPIS.xlsx)
