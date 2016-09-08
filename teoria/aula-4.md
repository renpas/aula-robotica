#Sensor ultrassônico

Este tipo de sensor serve para medir distância.

Este sensor retorna um valor que varia de 0 à 100 centímetros.
	
##Exemplo (pg. 21 tutorial):
```c
	#define NEAR 22

    task main(){
        SetSensorLowspeed(IN_4);
        while(true){
            OnFwd(OUT_AC, 50);
            while(SensorUS(IN_4) > NEAR);
            Off(OUT_AC);
            OnRev(OUT_C, 10);
            Wait(800);
        }
    }
```
