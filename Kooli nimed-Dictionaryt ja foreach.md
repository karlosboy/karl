static void Main(string[] args)
        {
            Console.WriteLine("Kooli nimed");

            Dictionary<int, string> schools = new Dictionary<int, string>();
            {
                schools.Add(1, "Viimsi Kool");
                schools.Add(2,"Pirita Kool");
                schools.Add(3, "Pärnu Kool");
            };


            foreach (KeyValuePair<int, string> school in schools)
            {
                Console.WriteLine("Kool #" + school.Key + ":  " + school.Value);
            }
        }
    }
}

        
