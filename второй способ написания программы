 class Program
        {
            static void Main(string[] args)
            {
                double a, b, c;
                a = enter();
                b = enter();
                c = enter();
                var (x1, x2, x) = First(a, b, c);
                if (x == 0)
                {
                    Console.ForegroundColor = ConsoleColor.Red;
                    Console.WriteLine("Действительных корней нет");
                    Console.ForegroundColor = ConsoleColor.White;
                    Environment.Exit(0);
                }
                else
                if (x1 < 0 && x2 < 0)
                {
                    Console.ForegroundColor = ConsoleColor.Red;
                    Console.WriteLine("Действительных корней нет");
                    Console.ForegroundColor = ConsoleColor.White;
                    Environment.Exit(0);
                }
                else if ((x1 < 0) && (x2 > 0))
                {
                    double xx1 = Math.Sqrt(x2);
                    double xx2 = -Math.Sqrt(x2);
                    Console.ForegroundColor = ConsoleColor.Green;
                    Console.Write($"X1 = {xx1} X2 = {xx2} ");
                    Console.ForegroundColor = ConsoleColor.White;
                    Environment.Exit(0);

                }
                else if ((x1 > 0) && (x2 < 0))
                {
                    double xx1 = Math.Sqrt(x1);
                    double xx2 = -Math.Sqrt(x1);
                    Console.ForegroundColor = ConsoleColor.Green;
                    Console.Write($"X1 = {xx1} X2 = {xx2} ");
                    Console.ForegroundColor = ConsoleColor.White;
                    Environment.Exit(0);
                }
                else
                {
                    double xx1 = Math.Sqrt(x1);
                    double xx2 = -Math.Sqrt(x1);
                    double xx3 = Math.Sqrt(x2);
                    double xx4 = -Math.Sqrt(x2);
                    Console.ForegroundColor = ConsoleColor.Green;
                    Console.Write($"X1 = {xx1} X2 = {xx2} X3 = {xx3} X4 = {xx4} ");
                    Console.ForegroundColor = ConsoleColor.White;
                    Environment.Exit(0);


                }
            } // Выделение корней
            static double enter()
            {
                while (true)
                    try
                    {
                        return Convert.ToDouble(Console.ReadLine());
                    }
                    catch
                    {
                        Console.WriteLine(" Ммм,бро, а шо это за символы такие?!");
                    }
            } // Проверка на вшивость
            private static (double x1, double x2, int x) First(double a, double b, double c) // Квадратное уравнение
            {

                double D = b * b - 4 * a * c;
                double x1 = (-b + Math.Sqrt(D)) / (2 * a);
                double x2 = (-b - Math.Sqrt(D)) / (2 * a);
                if (D < 0)
                {
                    int x = 0;
                    var result1 = (x1, x2, x);
                    return result1;

                }
                else
                {
                    int x = 1;
                    var result1 = (x1, x2, x);
                    return result1;
                }
            }
        }
