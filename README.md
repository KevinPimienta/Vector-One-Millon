# Vector-One-Millon
Tiempo de ejecución.

decimal Suma = 0;
            decimal[] Vektor = new decimal[100];
            Random random = new Random();
                TimeSpan stop;
                TimeSpan start = new TimeSpan(DateTime.Now.Ticks);
            for (int n = 0; n < Vektor.Length; n++)
            {
                Vektor[n] = random.Next(1, 1000000);
                Console.WriteLine(Vektor[n]);
                Suma = Suma + Vektor[n];  
            }
                stop = new TimeSpan(DateTime.Now.Ticks);
            Console.WriteLine();
            Console.Write("Tiempo de ejecución: "); Console.WriteLine(stop.Subtract(start).TotalSeconds);
            Console.Write("La suma es: " + Suma);
            Console.ReadKey();
