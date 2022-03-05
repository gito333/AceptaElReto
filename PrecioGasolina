package PrecioGasolina;

import java.util.Scanner;

public class PrecioGas {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        System.out.println();
        int dias = in.nextInt();
        while (dias != 0) {
            int diasConMas = 0;
            int[] arrayDias = new int[dias];
            for (int i = 0; i < dias; i++) {
                arrayDias[i] = in.nextInt();
            }
            for (int k = 0; k<dias;k++){
                int counter = 1;
                int mayor = k;
                for(int j = k;j<dias;j++){
                        if(arrayDias[j]>arrayDias[mayor]){
                            counter++;
                            mayor = j;
                        }
                }

                if(counter>diasConMas){
                    diasConMas = counter;
                }
            }
            System.out.println(diasConMas);
            dias = in.nextInt();
        }
    }
}
