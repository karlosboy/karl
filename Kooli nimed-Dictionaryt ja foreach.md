static void Main(string[] args)
        {
            
            Dictionary<string, int> schoolNames = new Dictionary<string, int>();
            schoolNames.Add("Laagna Kool", 12345);
            schoolNames.Add("Mustamäe Kool", 54321);
            schoolNames.Add("Viimsi Kool", 98765);

            
            foreach (KeyValuePair<string, int> school in schoolNames)
            {
                Console.WriteLine(school.Key + ": " + school.Value);
            }
        }
    }
}



