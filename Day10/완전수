using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace PerfertNumber
{
    internal class Program
    {
        static bool IsPerfectNumber(int num)
        {
            // 약수의 합을 계산합니다.
            int sum = 0;
            for (int i = 1; i <= num / 2; i++)
            {
                if (num % i == 0)
                {
                    sum += i;
                }
            }

            // 약수의 합이 주어진 숫자와 같은지 확인합니다.
            if (sum == num)
            {
                return true;  // 완전수입니다.
            }
            else
            {
                return false;  // 완전수가 아닙니다.
            }
        }
        static void Main(string[] args)
        {
            int num = Convert.ToInt32(Console.ReadLine());

            // 완전수 여부를 판별합니다.
            bool isPerfect = IsPerfectNumber(num);

            // 결과를 출력합니다.
            if (isPerfect)
            {
                Console.WriteLine("Yes");
            }
            else
            {
                Console.WriteLine("No");
            }
        }
    }
}
