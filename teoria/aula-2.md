#Sensor de toque

É o sensor mais simples de usar, pois retorna somente os valores 0 ou 1, ou seja:

0 - quando não há toque
1 - quando tocado.
	
##Exemplo (pg. 18 tutorial):
```
	task main(){
		SetSensor(In_1, Sensor.TOUCH);
		OnFwd(OUT_AC, 75);
		until(Sensor.1 == 1);
		Off(OUT_AC);
	}
```
