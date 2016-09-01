#Sensor de som

Este tipo de sensor capta o som externo no robô.

O som é captado em db (decibéis).

Este sensor retorna valores de 0 à 100.
	
##Exemplo (pg. 21 tutorial):
```c
	#define THRESHOLD 90
	#define mic SENSOR_2
	
	task main(){
		SetSensorSound(IN_2);
		while(true){
			until(mic > THRESHOLD);
			OnFwd(OUT_AC, 75);
			Wait(300);
			until(mic > THRESHOLD);
			Off(OUT_AC);
			Wait(300);

		}
	}
```
