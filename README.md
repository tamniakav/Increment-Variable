# Increment-Variable
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _6.Increment_Variable
{
    class Program
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());
            int overFlowed = 0;            
            byte count = 0;

            if (n <= byte.MaxValue)
            {
                Console.WriteLine(n);
            }
            else
            {

                for (int i = 1; i <= n; i++)
                {
                    count++;
                    
                    if (count == 0)
                    {                       
                        overFlowed++;
                    }
                }
                Console.WriteLine(count);
                Console.WriteLine($"Overflowed {overFlowed} times");
            }

        }
    }
}
