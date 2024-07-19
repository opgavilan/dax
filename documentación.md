# Documentación
## HASONEVALUE
### Escenario 1. HASONEVALUE+SEGMENTACIÓN DE DATOS
Para este escenario el HASONEVALUE, es aplicado con la segmentación de datos, ya que esta haciendo referencia a la columna [Tipo Escenario] de la tabla parametros, donde si es único, podremos aplicar la siguiente operación. Los valores de [porcentaje.decimal], ayudan en dar un proyectado sobre la medida [VentaTotal].

```
=IF(HASONEVALUE(parametros[Tipo Escenario]);    
	[VentaTotal]*    
 (1+VALUES(parametros[porcentaje.decimal]));    
	BLANK()    
 )
```
[img1][https://github.com/user-attachments/assets/fee2b1ce-0f09-4f9f-a0a6-ac67bf1eff45]
![image](https://github.com/user-attachments/assets/0ae6f5ae-d1bb-49dc-ad1a-848b221b7e5e)


<img src="https://github.com/user-attachments/assets/fee2b1ce-0f09-4f9f-a0a6-ac67bf1eff45" width="200" height="200"> <img src="https://github.com/user-attachments/assets/0ae6f5ae-d1bb-49dc-ad1a-848b221b7e5e" width="200" height="200">



 
