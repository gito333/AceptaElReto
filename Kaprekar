package kaprekar;

import java.util.Scanner;

public class Kaprekar {
    static Scanner in = new Scanner(System.in);

    public static void main(String[] args) {
        int iteraciones = in.nextInt();
        for (int i = 0; i < iteraciones; i++) {
            int counter = 0;
            int numero = in.nextInt();
            while(numero != 6174){
                numero = func(numero);
                if(numero == 0) {
                    numero =6174;
                    counter = 7;
                }
                counter++;
            }
            System.out.println(counter);
        }
    }

    public static int func(int number) {
        int[] restos = new int[4];
        for (int k = 0; k < 4; k++) {
            restos[k] = number % 10;
            number = number / 10;
        }
        for (int j = 0; j < 4; j++) {
            for (int k = 0; k < 4; k++) {
                int aux = 0;
                if (restos[j] < restos[k]) {
                    aux = restos[j];
                    restos[j] = restos[k];
                    restos[k] = aux;
                }
            }
        }
        int num1 = 0;
        int num2 =0;
        int j =3;
        for(int k = 0;k<4; k++){
            num1 += restos[j] * Math.pow(10,k);
            num2 += restos[k] * Math.pow(10,k);
            j--;
        }
        return num2-num1;
   }
}
