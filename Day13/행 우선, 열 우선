using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace TwoArrayApp01
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int[,] arr = new int[3, 4];
            string[] input = Console.ReadLine().Split(' ');

            // 행 우선으로 입력
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    arr[i, j] = int.Parse(input[i * 4 + j]);
                }
            }

            // 3행 4열로 출력 합시다.
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 4; j++)
                {
                    Console.Write(arr[i, j] + " ");
                }
                Console.WriteLine();
            }
            Console.WriteLine();

            // 4행 3열로 출력 합시다.
            for (int j = 0; j < 4; j++)
            {
                for (int i = 0; i < 3; i++)
                {
                    Console.Write(arr[i, j] + " ");
                }
                Console.WriteLine();
            }

        }
    }
}
