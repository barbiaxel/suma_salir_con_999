# suma_salir_con_999
Realiza un programa que sume un conjunto de valores introducidos por teclado hasta introducir el valor 999 (no sumar este valor, indica que ha finalizado la introducción de valores). Se debe mostrar el valor de la suma y decir si dicho valor es cero, mayor a cero o menor a cero.
import java.util.Scanner;

public class SumaValores {

	public static void main(String[] args) {
		Scanner teclado = new Scanner(System.in);
		int suma = 0, valor;
		do {
			System.out.println("Introduce un valor:");
			valor=teclado.nextInt();
			if (valor!=999) {
				suma= suma+valor;
			}	
		} while (valor!=999);
		
		System.out.println("Suma acumulada:" +suma);
		if (suma==0) {
			System.out.println("la suma es cero");
		} else {
			if (suma>0) {
				System.out.println("La suma es positiva");
			} else {
				System.out.println("La suma es negativa");
			}
		}
	}

}
