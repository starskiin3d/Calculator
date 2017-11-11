# Calculator
MS DoS Calculator
namespace Two_numbers
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                int number1;
                string operant;
                int number2;

                Console.Write("Enter first number: ");
                number1 = Convert.ToInt32(Console.ReadLine());
                Console.Write("Enter Operant EG: +,-,*,/: ");
                operant = Console.ReadLine();
                Console.Write("Enter second number: ");
                number2 = Convert.ToInt32(Console.ReadLine());
                Console.WriteLine("Good Day {0}", DateTime.Now);
                switch (operant)

                {
                    case "+":
                        Console.WriteLine("The Result Of {0} + {1} = {2}", number1, number2, number1 + number2);
                        break;

                    case "-":
                        Console.WriteLine("The Result Of {0{ * {1} = {2}", number1, number2, number1 - number2);
                        break;

                    case "*":
                        Console.WriteLine("The result of [0} * {1} = {2}", number1, number2, number1 * number2);
                        break;

                    case "/":
                        Console.WriteLine("The result of {0} / {1} = {2}", number1, number2, number1 / number2);
                        break;

                    case "_":
                        Console.WriteLine("Wrong operant _ switching to - instead {0} - {1} = {2}", number1, number2, number1 - number2);
                        break;

                    case "=":
                        Console.WriteLine("Wrong operant = switching to + instead {0} + {1} = {2}", number1, number2, number1 + number2);
                        break;
                }
            }
            catch (Exception)
            {
                Console.WriteLine("Exception wrong input try again!!");
            }
        }

    }
      }
