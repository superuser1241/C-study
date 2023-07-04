using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace CatApp01
{
    class Dog
    {
        private string name;
        public Dog(string _name)
        {
            name = _name;
        }
        public string getName()
        {
            return name;
        }
        public string Eat()
        {
            return "먹습니다.";
        }
        public string Play()
        {
            return "뛰어놀다";
        }
    }
    internal class Program
    {
        static void Main(string[] args)
        {
            Dog tom = new Dog("톰");
            Console.WriteLine($"{tom.getName()}이 음식을 {tom.Eat()}");
            Console.WriteLine($"{tom.getName()}이 {tom.Play()}");

        }
    }
}
