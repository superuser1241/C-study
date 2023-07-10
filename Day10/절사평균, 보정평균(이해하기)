using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Quiz20
{

    internal class Program
    {
        static void Main(string[] args)
        {
            string[] input = Console.ReadLine().Split();
            int N = int.Parse(input[0]);    //입력값 수
            int K = int.Parse(input[1]);    //제외되는 값

            //처음 테스트 할때는 입력을 받지말고 상수값으로 만든 후 테스트 
            // int N = 7;  
            // int K = 2;

            //점수 입력받기
            double[] score = new double[N];
             for(int i=0; i<N; i++)
             {
                 score[i] = double.Parse(Console.ReadLine());
             }
            //처음 테스트 할때는 입력을 받지말고 상수값으로 만든 후 테스트    
            //double[] score = { 9.3, 9.5, 9.6, 9.8, 9.1, 5.0, 9.3 };

            //정렬하기
            Array.Sort(score);

            //절사평균
            double trimmedMean = 0;
            for (int i = K; i < N - K; i++)
            {
                trimmedMean += score[i];
            }
            trimmedMean /= (N - (K * 2)); //(K*2)인 이유는 양쪽에서 빼기때문에 x2

            //보정평균
            double adjustedMean = 0;
            for (int i = 0; i < K; i++)
            {
                adjustedMean += score[K]; //K개의 점수를 모두 같은 점수로 보정한 후  더함
            }
            for (int i = K; i < N - K; i++) //중간 부분의 점수만 구함, 보정없이 그대로 사용
            {
                adjustedMean += score[i];
            }
            for (int i = N - K; i < N; i++) //뒷쪽 K개의 점수를 모두 같은 점수(뒤에서 K번째 점수)로 보정한 후 이를 더합니다. 
            {
                adjustedMean += score[N - K - 1];
            }
            adjustedMean /= N; //평균구하기 실수/정수 -> 실수

            Console.WriteLine($"{trimmedMean:F2}"); //절사평균
            Console.WriteLine($"{adjustedMean:F2}"); //보정평균
        }
    }
}
 
