Lego mindstorms

Linguagem de programa��o: NXC, ou seja, linguagem C com comandos do lego.

A CPU do lego � chamada de NXT, e � l� que fica��o armazenados nossos programas.

Ser� utilizado o programa BRCX Command Center para programar ou compilar, mas antes de abrir este software � necess�rop ligar o rob� e conectar na porta USB do computador.

#Comandos B�sicos:

	onfwd(OUT_AC, 70);
		liga os motores A eC para frente com velocidade de 70%
	
	off(OUT_AC);
		Desliga os motores A e CPU
	
	onrev(OUT_B, 50);
		Reverte o motor B com velocidade de 50%
		
	wait(2000);
		Executa o comando anterior por 2000 mil�simos de segundos antes de executar o pr�ximo comando
	
Exemplo:
	task main(){
		onfwd(OUT_AC, 75);
		wait(3000);
		onrev(OUT_C, 50);
		wait(1000);
		off(OUT_AC);
	}
	