using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Dictionary_CheckLogin
{
    internal class Program
    {
        static string CheckLogin(Dictionary<string, string> userInfo, string id, string pwd)
        {
            if (userInfo["userId"] == id && userInfo["password"] == pwd)
            {
                return "로그인에 성공했습니다.";
            }
            else
            {
                return "로그인에 실패했습니다.";
            }
        }
        static void Main(string[] args)
        {
            Dictionary<string, string> userInfo = new Dictionary<string, string>
            {
                {"userId", "admin"},
                {"password", "1234"}
            };

            string id, pwd;

            Console.Write("ID를 입력하세요: ");
            id = Console.ReadLine();

            Console.Write("패스워드를 입력하세요: ");
            pwd = Console.ReadLine();

            Console.WriteLine(CheckLogin(userInfo, id, pwd));
        }
    }
}
