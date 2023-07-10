using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace OddMagicSquare
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.Write("N: ");
            int N = int.Parse(Console.ReadLine());

            if (N % 2 == 0)
            {
                Console.WriteLine("N은 홀수만 가능합니다.");
                Environment.Exit(0);
            }

            int[,] magicSquare = new int[N, N]; //N이 입력된 상태라 크기가 결정됨
                                            //그리고 c#배열은 만들어지면 0으로 초기화 되어있다.
            int y = 0; //첫값의 y는 0
            int x = N / 2; //첫째줄 x값 정하기

            for (int i = 1; i <= N * N; i++) //N*N 마방진 크기
            {
                magicSquare[y, x] = i; // i는 채워넣는 카운트

                int tempX = (x + 1) % N; 
                int tempY = (y - 1 >= 0) ? y - 1 : N - 1; //조건이 참이면 y-1 아니면 N-1

                if (magicSquare[tempY, tempX] != 0) // 0이 아니라면 값을 넣을 수 없다.
                {
                    y = (y + 1) % N;
                }
                else
                {
                    x = tempX;  //tempX가 0인 상태라 값을 넣을 수 있다.
                    y = tempY;  
                }
            }//end of for --> 마방진 생성조건

            //마방진이 메모리엔 그려졌지만 이제 콘솔에서 그리기
            for (int i = 0; i < N; i++)
            {
                for (int j = 0; j < N; j++)
                {
                    Console.Write(magicSquare[i, j] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
