Lego mindstorms

Linguagem de programação: NXC, ou seja, linguagem C com comandos do lego.

A CPU do lego é chamada de NXT, e é lá que ficação armazenados nossos programas.

Será utilizado o programa BRCX Command Center para programar ou compilar, mas antes de abrir este software é necessárop ligar o robô e conectar na porta USB do computador.

#Comandos Básicos:

	onfwd(OUT_AC, 70);
		liga os motores A eC para frente com velocidade de 70%
	
	off(OUT_AC);
		Desliga os motores A e CPU
	
	onrev(OUT_B, 50);
		Reverte o motor B com velocidade de 50%
		
	wait(2000);
		Executa o comando anterior por 2000 milésimos de segundos antes de executar o próximo comando
	
Exemplo:
```
	task main(){
		onfwd(OUT_AC, 75);
		wait(3000);
		onrev(OUT_C, 50);
		wait(1000);
		off(OUT_AC);
	}
```
