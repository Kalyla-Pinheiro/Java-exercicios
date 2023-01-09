# Java-exercicios
Resolução

import java.util.Scanner;

public class Main {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		System.out.println("INSIRA A HORA INICIAL E A HORA FINAL DE UM JOGO: ");

		int horaInicial, horaFinal, duracao;

		horaInicial = sc.nextInt();
		horaFinal = sc.nextInt();
	

		if (horaInicial < horaFinal) {
			duracao = horaFinal - horaInicial;
		}

		else {
			duracao = 24 - (horaInicial - horaFinal);
		}

		System.out.println("O JOGO DUROU " + duracao + " HORA (S) ");
		sc.close();
	}

}
