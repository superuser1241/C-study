using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace FactorialApp01
{
    class Calculator
    {
        //점화식-일종의 다이나믹
        public int Factorial(int n)
        {
            int result = 1;
            for (int i = 2; i <= n; i++)
            {
                result *= i;
            }
            return result;
        }
        //재귀
        public int FactorialRecursive(int n)
        {
            if (n == 0)
                return 1;  
            else
                return n * Factorial(n - 1);  
        }

        //다이나믹
        public int FactorialDynamic(int n, int[] dp)
        {
            if (n == 0)
                return dp[n] = 1;

            if (dp[n] != 0)
                return dp[n];

            return dp[n] = n * FactorialDynamic(n - 1, dp);
        }

    }
    internal class Program
    {
        static void Main(string[] args)
        {
            int number = 5;
            Calculator calculator = new Calculator();
            int fact = calculator.Factorial(number);
            Console.WriteLine($"{number}의 팩토리얼은 {fact}입니다.");
            fact = calculator.FactorialRecursive(number);
            Console.WriteLine($"재귀적 방법을 이용한 {number}의 팩토리얼은 {fact}입니다.");
            int[] dp = new int[number + 1];
            fact = calculator.FactorialDynamic(number, dp);
            Console.WriteLine($"재귀적 방법을 이용한 {number}의 팩토리얼은 {fact}입니다.");

        }
    }
}
