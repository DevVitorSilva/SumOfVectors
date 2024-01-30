## Sum of Vectors

Faça um programa para ler dois vetores A e B, contendo N elementos cada. Em seguida, gere um terceiro vetor C onde cada elemento de C é a soma dos elementos correspondentes de A e B. imprima o vetor C gerado.

```java
import java.util.Locale;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Locale.setDefault(Locale.US);
        Scanner sc = new Scanner(System.in);
        System.out.print("How many values will each vector have? ");
        int quantity = sc.nextInt();
        int[] firstVector = new int[quantity];
        int[] secondVector = new int[quantity];
        System.out.println("Enter the value of vector A:");
        for(int i = 0; i < quantity; i++){
            System.out.print("Enter value here: ");
            firstVector[i] = sc.nextInt();
        }
        System.out.println("Enter the value of vector B:");
        for(int i = 0; i < quantity; i++){
            System.out.print("Enter value here: ");
            secondVector[i] = sc.nextInt();
        }
        int[] thirdVector = new int[quantity];
        System.out.println("Value of third vector: ");
        for(int i = 0; i < quantity; i++){
            thirdVector[i] = firstVector[i] + secondVector[i];
            System.out.println(thirdVector[i]);
        }
        sc.close();
    }
}
```