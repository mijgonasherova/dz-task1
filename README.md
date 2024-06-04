// Задача 1: Задайте значения M и N. Напишите программу, которая 
// выведет все натуральные числа в промежутке от M до N. 
// Использовать рекурсию, не использовать циклы.
// Пример
// M = 1; N = 5 -> "1, 2, 3, 4, 5"
// M = 4; N = 8 -> "4, 5, 6, 7, 8"

static void PrintNaturalNumbers(int M, int N)
{
    if (M <= N)
    {
        Console.Write(M + ", ");
        PrintNaturalNumbers(M + 1, N);
    }
}  

Console.Write("Введите натуральное число M: ");
int M = Convert.ToInt32(Console.ReadLine());

Console.Write("Введите натуральное число N: ");
int N = Convert.ToInt32(Console.ReadLine());

PrintNaturalNumbers(M, N);
Console.WriteLine();
