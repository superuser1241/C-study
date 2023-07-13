using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ExceptionApp01
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int[] arr = { 1, 2, 3 };

            try
            {
                //1.예외
                /*    for (int i = 0; i < 5; i++)
                    {
                        Console.WriteLine(arr[i]);
                    }
                */
                //2.예외
                int a = 100;
                int result = a / 0;

            }
            catch(IndexOutOfRangeException e)
            {
                Console.WriteLine("배열의 범위를 벗어난 예외가 발생하였습니다.");
                Environment.Exit(0);
            }
            catch(DivideByZeroException e)
            {
                Console.WriteLine("0으로 나누면 안됩니다.");
                Environment.Exit(0);
            }
            catch(Exception ex) 
            {
                Console.WriteLine(ex.Message);
                Environment.Exit(0);
            }
            

            Console.WriteLine("종료");
        }
    }
}
