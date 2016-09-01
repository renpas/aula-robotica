#Sensor de toque

É o sensor mais simples de usar, pois retorna somente os valores 0 ou 1, ou seja:

0 - quando não há toque
1 - quando tocado.
	
##Exemplo (pg. 18 tutorial):
```c
	task main(){
		SetSensor(IN_1, SENSOR_TOUCH);
		OnFwd(OUT_AC, 75);
		until(SENSOR_1 == 1);
		Off(OUT_AC);
	}
```
