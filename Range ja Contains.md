namespace ConsoleApp5
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Range and Contains TÖÖ");

            //kutsume RangeLINQ meetoidi välja ja ContainsLINQ
            RangeLINQ();
            ContainsLINQ();
        }

        public static void RangeLINQ()
        {
            // Loob täisarvude jada vahemikus 1 kuni 10
            // ja seejärel valib nende ruudud.
            IEnumerable<int> squares = Enumerable.Range(1, 10).Select(x => x * x);

            foreach (int num in squares)
            {
                Console.WriteLine(num);
            }

            /*
             See kood annab järgmise väljundi:

             1
             4
             9
             16
             25
             36
             49
             64
             81
             100
            */
        }

       
        public static void ContainsLINQ()
        {
            string str = "I love ice cream";

            bool check;

            // kontrollib, kas str sisaldab "jäätist"
            check = str.Contains("ice cream");
            Console.WriteLine("contains ice cream: " + check);

            // kontrollib, kas str sisaldab sõna "šokolaad"
            check = str.Contains("chocolate");
            Console.WriteLine("contains chocolate: " + check);

            // tagastab tõele
            check = str.Contains("");
            Console.WriteLine("contains \"\": " + check);

            Console.ReadLine();
        }
    }
}
