# Documentación
## HASONEVALUE
Para este escenario el HASONEVALUE, es aplicado con la segmentación de datos, ya que esta esta haciendo referencia a la columna [Tipo Escenario] de la tabla parametros, donde si es único, podremos aplicar la siguiente operación. Los valores de [porcentaje.decimal], ayudan en dar un proyectado sobre la medida [VentaTotal].

```
=IF(HASONEVALUE(parametros[Tipo Escenario]);    
	[VentaTotal]*    
 (1+VALUES(parametros[porcentaje.decimal]));    
	BLANK()    
 )
```

![image](https://github.com/user-attachments/assets/fee2b1ce-0f09-4f9f-a0a6-ac67bf1eff45)


 
