```c#

using System;
namespace Abcde
{
    class Program
    {
        static void Main(string[] args)
        {
            Test obj = new Test();
            obj.title();

            int[] arr = { 10, 27, 23, 3, 34, 12, 5, 6 };
            Console.WriteLine(obj.min(arr));

            obj.twoArrays(2,3);

            for (int i = 0; i < arr.Length;  i++)
            {
                Console.WriteLine($"{i} Wert={arr[i]}");
            }

            Console.ReadKey();
        }
    }
}

```

```c#
using System;
using System.Collections.Generic;
using System.Text;

namespace Abcde
{
    class Test
    {
        public void title()
        {
            Console.Write("Die kleinste Wert ist: ");
        }

        public void twoArrays(int i, int j)
        {
            int[,] zahlen =
            {
                {1,2,3,4},
                {5,6,7,8 },
                {9,10,11,12}
            };

            Console.WriteLine(zahlen[i, j]);
        }

        public int min(int[] liste)
        {
            int min = liste[0];

            for (int i = 0; i < liste.Length; i++)
            {
                if (liste[i] <= min)
                {
                    min = liste[i];

                }
            }

            return min;
        }

        public void isArrayDynamisch(int[] arr)
        {
            if (arr.Length > 0 && arr.Length < 1000)
            {
                Console.WriteLine($"Array ist dynamish: i={arr.Length}");
            }
            else
            {
                Console.Error.WriteLine("Diese Array ist nicht dynamisch!");
            }
        }

    }
}

 ´´´
