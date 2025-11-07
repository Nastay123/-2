using System;

public class DifferenceCalculator
{
    public static int CalculateDifference(int n)
    {
        int targetNumber = 123;
        int difference = Math.Abs(n - targetNumber); 

        if (n > targetNumber)
        {
            return difference * 3; 
        }
        else
        {
            return difference; 
        }
    }
    public static void Main(string[] args)
    {
        Console.WriteLine(" Расчет абсолютной разности ");

        int num1 = 150;
        int diff1 = CalculateDifference(num1);
        Console.WriteLine($"Для n = {num1}: Абсолютная разность = {diff1}");
        int num2 = 100;
        int diff2 = CalculateDifference(num2);
        Console.WriteLine($"Для n = {num2}: Абсолютная разность = {diff2}"); 

        int num3 = 123;
        int diff3 = CalculateDifference(num3);
        Console.WriteLine($"Для n = {num3}: Абсолютная разность = {diff3}"); 

        Console.WriteLine("\nНажмите любую клавишу для выхода...");
        Console.ReadKey();
    }
}
