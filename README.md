# QUESTION-NO-1


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp13
{
    class Program
    {
        public static void Main(string[] args)
        { 
        
           int count=0;
            int fact = 1;
            Console.WriteLine("Enter a Number:");
            int num = int.Parse(Console.ReadLine());
            if(num<=0)
            {
                Console.WriteLine("Enter positive Number only:");
               
            }
            else
            {
                for (int i = 1; i <= num; i++)
                {
                    if (num % i == 0)
                    {
                        count++;
                    }
                }
                    if(count==2)
                    {
                        Console.WriteLine("{0} Number is Prime.\n",num);
                    for (int j = 1; j <=num; j++)
                    {
                        fact = fact * j;
                    }
                    Console.WriteLine("The factorial of Number is:"+fact);
                    }
                    else
                    {
                        Console.Write("{0} Number is not Prime.\n",num);
                    int a = 0;
                    int b = 1;
                    int c;
                    Console.WriteLine("Here is fabonacci series of Number {0} :",num);
                    Console.WriteLine(a);
                    Console.WriteLine(b);
                    for (int k = 0; k <=10; k++)
                    {
                        c = a + b;
                        Console.WriteLine(c);
                        a = b;
                        b = c;
                    }
                    }                                       
            }
            Console.ReadLine();
        }
    }
}
