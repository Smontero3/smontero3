\\ Leer un número entero de dos dígitos y determinar a cuánto es igual la suma de sus dígitos.
using System;


public class Exercise27 {

    public static void Main() {
        Console.Write("Ingrese un numero de 2 digitos: "); 

        int n = Convert.ToInt32(Console.ReadLine()); 

        int sum = 0; 
     
        while (n != 0) {
            sum += n % 10; 
            n /= 10; 
        }

        Console.WriteLine("La suma de los digitos es: " + sum);
    }
}
