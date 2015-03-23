# Trivia-Quiz
C# class

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace dan_s_trivia_game
{
    public class Program
    {

        static int score1 = 0;
        static int score2 = 0;
        static int score;
        static bool name = true;


        public static class Name
        {
            public static string name;
            public static string name2;
        }

        public static class AnswerChoices
        {

            public static string B;
            public static string D;
            public static string A;
            public static string C;
            public static string E;

        }

        public static void Introduction()
        {
            // Introduction to the game

            Console.Write("please input your name player 1 ");
            Name.name = Console.ReadLine();
            Console.Clear();

            Console.Write("please input your name player 2 ");
            Name.name2 = Console.ReadLine();
            Console.Clear();
            Console.WriteLine(Name.name + " You  will answer a series of trivia questions, the topics include are, Nintendo, Playstation, Xbox, Sega, Random Video Game trivia");
            Console.SetCursorPosition(0, 4);
            Console.ReadLine();
            Console.WriteLine("You will have a time limit however to answer the questions and now turn on your Caps Lock ;)");
            Console.WriteLine("Also after you answer 5 questions you can  end the game");
            Console.WriteLine("Pssh, keep your CMD open for continue, Thank you");
            Console.ReadLine();

        }

        public static void FirstNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "1) What was the initial name for the first Super Smash Bros?");
            Console.WriteLine("A:Nintendo Brawl");
            Console.WriteLine("B:Dragon King: The fighting Game");
            Console.WriteLine("C:End: World Tournament");
            Console.WriteLine("D:Survival");
            Console.WriteLine("E:Exit");
            string B = Console.ReadLine();
            if (B == "B")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + " That is the correct answer. Your score is " + score);
                Console.ReadLine();
                SecondNintendoQuestion();
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            FirstNintendoQuestion();
        }

        public static void SecondNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "2) Who were the four nintendo characters Sakurai used to get Nintendo to use their characters in Super Smash Bros.?");
            Console.WriteLine("A:Samus, Mario, Luigi, Fox");
            Console.WriteLine("B:Mario, Luigi, Peach, Bowser");
            Console.WriteLine("C:Falco, Fox, Donkey Kong, Mario");
            Console.WriteLine("D:Mario, Samus, Fox, Donkey Kong");
            Console.WriteLine("E:Exit");
            string D = Console.ReadLine();
            if (D == "D")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "Correct answer. Your score is " + score);
                Console.ReadLine();
                ThirdNintendoQuestion();
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            SecondNintendoQuestion();
        }
        public static void ThirdNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "3) Which non-gaming console actually had nintendo games developed for it?");
            Console.WriteLine("A:Blu-Ray");
            Console.WriteLine("B:Philips CDI");
            Console.WriteLine("C:Apple home computers");
            Console.WriteLine("D:none of the above");
            Console.WriteLine("E:Exit");
            string B = Console.ReadLine();
            if (B == "B")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That right. Your score is " + score);
                Console.ReadLine();
                SecondNintendoQuestion();
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            FirstNintendoQuestion();
        }

        public static void FourthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "4) What game was the first one Mario appeared in? ");
            Console.WriteLine("A:Super mario Bros");
            Console.WriteLine("B:Yoshi Island");
            Console.WriteLine("C:Donkey Kong");
            Console.WriteLine("D:Donkey Kong 64");
            Console.WriteLine("E:Exit");
            string C = Console.ReadLine();
            if (C == "C")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "True. Your score is " + score);
                Console.ReadLine();
                FithNintendoQuestion();
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            FourthNintendoQuestion();
        }

        public static void FithNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "5)What Nintendo system is said to “have saved the entire gaming industry single handedly”?");
            Console.WriteLine("A:Gameboy");
            Console.WriteLine("B:Nintendo 64");
            Console.WriteLine("C:SNES");
            Console.WriteLine("D:NES");
            Console.WriteLine("E:Exit");
            string D = Console.ReadLine();
            if (D == "D")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "Gaming histry right there. Your right by the way. Your score is " + score);
                Console.SetCursorPosition(0,4);
                Console.ReadLine();
                SecondNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            FithNintendoQuestion();
        }

        public static void SixthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "6)How old was Sakurai when he invented one of the most popular video game characters ever, Kirby?");
            Console.WriteLine("A:16");
            Console.WriteLine("B:19");
            Console.WriteLine("C:21");
            Console.WriteLine("D:25");
            Console.WriteLine("E:Exit");
            string B = Console.ReadLine();
            if (B == "B")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                SeventhNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            SixthNintendoQuestion();
        }

        public static void SeventhNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + "7) How old is the Nintendo company?");
            Console.WriteLine("A:120yrs");
            Console.WriteLine("B:100yrs");
            Console.WriteLine("C:126yrs");
            Console.WriteLine("D:115yrs");
            Console.WriteLine("E:Exit");
            string C = Console.ReadLine();
            if (C == "C")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "Good Job. Your score is " + score);
                Console.ReadLine();
                EigthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            SeventhNintendoQuestion();
        }

        public static void EigthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 8) Before the GameBoy released, which was the first handheld system Nintendo developed?");
            Console.WriteLine("A:gameboy was the 1st");
            Console.WriteLine("B:DS");
            Console.WriteLine("C:Game and Watch");
            Console.WriteLine("D:None of the above");
            Console.WriteLine("E:Exit");
            string C = Console.ReadLine();
            if (C == "C")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "Yea. Your score is " + score);
                Console.ReadLine();
                NinethNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            EigthNintendoQuestion();
        }

        public static void NinethNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 9) Why was luigi designed to wear green?");
            Console.WriteLine("A:Its opposite to red on the color wheel");
            Console.WriteLine("B:It was easily distinguishable to be 2nd player in his 1st game");
            Console.WriteLine("C:The system restrictions made them re-use the color of an enemy");
            Console.WriteLine("D:the game developers favorite colors are red, white, and green");
            Console.WriteLine("E:Exit");
            string C = Console.ReadLine();
            if (C == "C")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "Technology must have sucked back then. he stole the green Koopa shell solors. Your score is " + score);
                Console.SetCursorPosition(0,4);
                Console.ReadLine();
                TenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            NinethNintendoQuestion();
        }


        public static void TenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 10) How did Nintendo get its start?");
            Console.WriteLine("A:making video games");
            Console.WriteLine("B:selling comics");
            Console.WriteLine("C:making stories");
            Console.WriteLine("D:a card and toy company");
            Console.WriteLine("E:Exit");
            string D = Console.ReadLine();
            if (D == "D")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                EleventhNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            TenthNintendoQuestion();
        }
        public static void EleventhNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 11) Which Nintendo game never released in the US due to religious reasons?");
            Console.WriteLine("A:the first Castlevania");
            Console.WriteLine("B:Dragon quest");
            Console.WriteLine("C:Devil World");
            Console.WriteLine("D:Silent hill");
            Console.WriteLine("E:Exit");
            string C = Console.ReadLine();
            if (C == "C")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                TwelfthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            EleventhNintendoQuestion();
        }
        public static void TwelfthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 12) How is Miyamoto forced to go to work every day at Nintendo?");
            Console.WriteLine("A:drive");
            Console.WriteLine("B:bus");
            Console.WriteLine("C:train");
            Console.WriteLine("D:bike");
            Console.WriteLine("E:Exit");
            string A = Console.ReadLine();
            if (A == "A")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                ThirteenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            TwelfthNintendoQuestion();
        }

        public static void ThirteenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 13) What was Kirby’s original name?");
            Console.WriteLine("A:no name");
            Console.WriteLine("B:Kirby");
            Console.WriteLine("C:Ray");
            Console.WriteLine("D:None of the above");
            Console.WriteLine("E:Exit");
            string D = Console.ReadLine();
            if (D == "D")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. His original name was actually Tinkle popo. You're laughing aren’t you? thats why they changed it..Your score is " + score);
                Console.SetCursorPosition(0, 4);
                Console.ReadLine();
                FourteenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            ThirteenthNintendoQuestion();
        }

        public static void FourteenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 14) What game was Luigi's first appearance?");
            Console.WriteLine("A:Super Mario Bros");
            Console.WriteLine("B:a Game and Watch game");
            Console.WriteLine("C:Luigi’s mansion");
            Console.WriteLine("D:none. He appeared in a cartoon first");
            Console.WriteLine("E:Exit");
            string B = Console.ReadLine();
            if (B == "B")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                FifteenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            FourteenthNintendoQuestion();
        }

        public static void FifteenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 15) Where did they get the voice of Marth from, for Super Smash Bros. Melee?");
            Console.WriteLine("A:The Fire Emblem Anime");
            Console.WriteLine("B:A voice actor recording new lines");
            Console.WriteLine("C:The Fire Emblem games themselves");
            Console.WriteLine("D:he has no lines");
            Console.WriteLine("E:Exit");
            string A = Console.ReadLine();
            if (A == "A")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                SixteenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            FifteenthNintendoQuestion();
        }

        public static void SixteenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 16) Which alien species appear in Kid Icarus uprising?");
            Console.WriteLine("A:Aliens from Alien");
            Console.WriteLine("B:Metroids from Metroid");
            Console.WriteLine("C:Coneheads from Coneheads");
            Console.WriteLine("D:ET from ET");
            Console.WriteLine("E:Exit");
            string B = Console.ReadLine();
            if (B == "B")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                SeventeenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            SixteenthNintendoQuestion();
        }

        public static void SeventeenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 17) From what game did a song that was from it, outsell the actual game release for a brief period of time?");
            Console.WriteLine("A:Pikman");
            Console.WriteLine("B:Starfox");
            Console.WriteLine("C:Metroid");
            Console.WriteLine("D:Super Mario Bros");
            Console.WriteLine("E:Exit");
            string A = Console.ReadLine();
            if (A == "A")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                Console.ReadLine();
                eightteenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is  " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            SeventeenthNintendoQuestion();
        }

               public static void eightteenthNintendoQuestion()
        {

            String NameSelect;
            if (name == true)
            {
                NameSelect = Name.name;
            }
            else
            {

                NameSelect = Name.name2;


            }
            Console.WriteLine(NameSelect + " 18) Which enemy will chase mario if u wait long enough, in super mario bros 3?");
            Console.WriteLine("A:Goombas");
            Console.WriteLine("B:Hammerbros");
            Console.WriteLine("C:Chain chomp");
            Console.WriteLine("D:Bowser");
            Console.WriteLine("E:Exit");
            string C = Console.ReadLine();
            if (C == "C")
            {
                if (name == true) { score1 = score1 + 1; score = score1; }
                else { score2 = score2 + 1; score = score2; }
                Console.WriteLine(Name.name + "Correct, wait for the chainchomp to pull 49 times, and the next time it will break free. Heres a tip: run. Your score is " + score);
                Console.SetCursorPosition(0, 4);
                Console.ReadLine();
                nineteenthNintendoQuestion(); // this is sixth nintendo question
            }
            string E = Console.ReadLine();
            if (E == "E")
                Results();
            else
                Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
            Name.name = Console.ReadLine();
            if (name == true)
                name = false;
            else name = true;
            Console.Clear();
            eightteenthNintendoQuestion();
        }

               public static void nineteenthNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 19) The wii sports golf courses are a reference to a game for which console?");
                   Console.WriteLine("A:NES");
                   Console.WriteLine("B:N64");
                   Console.WriteLine("C:N64");
                   Console.WriteLine("D:None, they are all original");
                   Console.WriteLine("E:Exit");
                   string A = Console.ReadLine();
                   if (A == "A")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                       Console.ReadLine();
                       twentythNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   nineteenthNintendoQuestion();
               }

               public static void twentythNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 20) Before mother 3 released on GameBoy, which system was it planned for?");
                   Console.WriteLine("A:NES");
                   Console.WriteLine("B:N64");
                   Console.WriteLine("C:Gmecube");
                   Console.WriteLine("D:SNES");
                   Console.WriteLine("E:Exit");
                   string B = Console.ReadLine();
                   if (B == "B")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "That is the correct answer. Your score is " + score);
                       Console.ReadLine();
                       twentyfirstNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentythNintendoQuestion();
               }

               public static void twentyfirstNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 21) True or false, Nintendo owns a sports team?");
                   Console.WriteLine("A:True");
                   Console.WriteLine("B:False");
                   Console.WriteLine("E:Exit");
                   string A = Console.ReadLine();
                   if (A == "A")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "That is the correct answer, the own the Seattle Miners. Your score is " + score);
                       Console.ReadLine();
                       twentysecondNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentyfirstNintendoQuestion();
               }

               public static void twentysecondNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 22) Which was a failed addon for the N64?");
                   Console.WriteLine("A:Microphone");
                   Console.WriteLine("B:Keyboard");
                   Console.WriteLine("C:Video player");
                   Console.WriteLine("D:Disk Drive");
                   Console.WriteLine("E:Exit");
                   string D = Console.ReadLine();
                   if (D == "D")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "Nice. Your score is " + score);
                       Console.ReadLine();
                       twentythirdNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentysecondNintendoQuestion();
               }

               public static void twentythirdNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 23) Other than the character, what does Smash Bros. have in common with kirby?");
                   Console.WriteLine("A:Same protagonist");
                   Console.WriteLine("B:Same voice actors for all characters");
                   Console.WriteLine("C:Same creator");
                   Console.WriteLine("D:Nothing at all,");
                   Console.WriteLine("E:Exit");
                   string C = Console.ReadLine();
                   if (C == "C")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "Nice. Your score is " + score);
                       Console.ReadLine();
                       twentyfourthNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentythirdNintendoQuestion();
               }

               public static void twentyfourthNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 24) What last minute addon helped to revolutionize FPS games today?");
                   Console.WriteLine("A:Goldeneye, Multiplayer");
                   Console.WriteLine("B:Quake, Single player");
                   Console.WriteLine("C:Super Mario Bros, 2 player gameplay");
                   Console.WriteLine("E:Exit");
                   string A = Console.ReadLine();
                   if (A == "A")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "Nice. Your score is " + score);
                       Console.ReadLine();
                       twentyfithNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentyfourthNintendoQuestion();
               }

               public static void twentyfithNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " 25) Back when they were a toy company, what other company did Nintendo rip-off for construction toys?");
                   Console.SetCursorPosition(0, 4);
                   Console.WriteLine("A:Minecraft");
                   Console.WriteLine("B:Lego ");
                   Console.WriteLine("C:Regular wooden blocks");
                   Console.WriteLine("D;None");
                   Console.WriteLine("E:Exit");
                   string B = Console.ReadLine();
                   if (B == "B")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "Good job. Your score is " + score);
                       Console.ReadLine();
                       twentysixthNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentyfithNintendoQuestion();
               }

               public static void twentysixthNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + " What was the code name for the GameCube?");
                   Console.SetCursorPosition(0, 4);
                   Console.WriteLine("A:Shark");
                   Console.WriteLine("B:Geo ");
                   Console.WriteLine("C:Dolphin");
                   Console.WriteLine("D;None");
                   Console.WriteLine("E:Exit");
                   string C = Console.ReadLine();
                   if (C == "C")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "Good job. Your score is " + score);
                       Console.ReadLine();
                       twentyseventhNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentysixthNintendoQuestion();
               }

          public static void twentyseventhNintendoQuestion()
               {

                   String NameSelect;
                   if (name == true)
                   {
                       NameSelect = Name.name;
                   }
                   else
                   {

                       NameSelect = Name.name2;


                   }
                   Console.WriteLine(NameSelect + "true or false: The palnnet koppai from pikan 3 is a reference to something?");
                   Console.SetCursorPosition(0, 4);
                   Console.WriteLine("A:True");
                   Console.WriteLine("B:False ");
                   Console.WriteLine("E:Exit");
                   string A = Console.ReadLine();
                   if (A == "A")
                   {
                       if (name == true) { score1 = score1 + 1; score = score1; }
                       else { score2 = score2 + 1; score = score2; }
                       Console.WriteLine(Name.name + "Good job. Nintendo Co. Ltd. was originally named Nintendo Koppai " + score);
                       Console.ReadLine();
                       twentyeighthNintendoQuestion(); // this is sixth nintendo question
                   }
                   string E = Console.ReadLine();
                   if (E == "E")
                       Results();
                   else
                       Console.WriteLine(Name.name + "Wrong, your turns up. Your score is " + score);
                   Name.name = Console.ReadLine();
                   if (name == true)
                       name = false;
                   else name = true;
                   Console.Clear();
                   twentyseventhNintendoQuestion();
               }

          public static void twentyeighthNintendoQuestion()
          {

              String NameSelect;
              if (name == true)
              {
                  NameSelect = Name.name;
              }
              else
              {

                  NameSelect = Name.name2;


              }
              Console.WriteLine(NameSelect + " Which company once made unofficial games for the NES?");
              Console.SetCursorPosition(0, 4);
              Console.WriteLine("A:Namco");
              Console.WriteLine("B:Bandai ");
              Console.WriteLine("C:Atari");
              Console.WriteLine("D;None");
              Console.WriteLine("E:Exit");
              string A = Console.ReadLine();
              if (A == "A")
              {
                  if (name == true) { score1 = score1 + 1; score = score1; }
                  else { score2 = score2 + 1; score = score2; }
                  Console.WriteLine(Name.name + "Yea, Namco actually made unofficial games for the NES because the company didn't like the game restrictions Nintendo placed. Your score is " + score);
                  Console.SetCursorPosition(0, 4);
                  Console.ReadLine();
                  twentyninethNintendoQuestion();
              }
              string E = Console.ReadLine();
              if (E == "E")
                  Results();
              else
                  Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
              Name.name = Console.ReadLine();
              if (name == true)
                  name = false;
              else name = true;
              Console.Clear();
              twentyeighthNintendoQuestion();
          }

          public static void twentyninethNintendoQuestion()
          {

              String NameSelect;
              if (name == true)
              {
                  NameSelect = Name.name;
              }
              else
              {

                  NameSelect = Name.name2;


              }
              Console.WriteLine(NameSelect + " Which company once made unofficial games for the NES?");
              Console.SetCursorPosition(0, 4);
              Console.WriteLine("A:Namco");
              Console.WriteLine("B:Bandai ");
              Console.WriteLine("C:Atari");
              Console.WriteLine("D;None");
              Console.WriteLine("E:Exit");
              string A = Console.ReadLine();
              if (A == "A")
              {
                  if (name == true) { score1 = score1 + 1; score = score1; }
                  else { score2 = score2 + 1; score = score2; }
                  Console.WriteLine(Name.name + "Yea, Namco actually made unofficial games for the NES because the company didn't like the game restrictions Nintendo placed. Your score is " + score);
                  Console.SetCursorPosition(0, 4);
                  Console.ReadLine();
                  thirtythNintendoQuestion();
              }
              string E = Console.ReadLine();
              if (E == "E")
                  Results();
              else
                  Console.WriteLine(Name.name + "That is not the correct answer. Your score is " + score);
              Name.name = Console.ReadLine();
              if (name == true)
                  name = false;
              else name = true;
              Console.Clear();
              twentyninethNintendoQuestion();
          }



























          static void Main(string[] args)
          {
              Program.Introduction();
              Program.FirstNintendoQuestion();
              Program.SecondNintendoQuestion();
              Program.ThirdNintendoQuestion();
              Program.FourthNintendoQuestion();
              Program.FithNintendoQuestion();
              Program.SixthNintendoQuestion();
              Program.SeventhNintendoQuestion();
              Program.EigthNintendoQuestion();
              Program.NinethNintendoQuestion();
              Program.TenthNintendoQuestion();
              Program.EleventhNintendoQuestion();
              Program.TwelfthNintendoQuestion();
              Program.ThirteenthNintendoQuestion();
              Program.FourteenthNintendoQuestion();
              Program.FifteenthNintendoQuestion();
              Program.eightteenthNintendoQuestion();
              Program.nineteenthNintendoQuestion();
              Program.twentythNintendoQuestion();
              Program.twentyfirstNintendoQuestion();
              Program.twentysecondNintendoQuestion();
              Program.twentythirdNintendoQuestion();
              Program.twentyfourthNintendoQuestion();
              Program.twentyfithNintendoQuestion();
              Program.twentysixthNintendoQuestion();
              Program.twentyseventhNintendoQuestion();




          }









            //Results Code

            public static void Results()
             {
            Console.WriteLine(" Your results are  ");
            Console.ReadLine();
            if (score1<score2)
            {
                Console.WriteLine(Name.name2 + " You are the Winner Congrats! You have " + score2 );
                Console.WriteLine(Name.name + " Better luck next time. You have " + score1);
                Console.ReadLine();
                Console.WriteLine(Name.name + " and ");
                Console.WriteLine(Name.name2+ " Thanks for playing my game. come back soon you hear? ");
                Console.ReadLine();

            }

                else if (score1>score2)
            {
                Console.WriteLine(Name.name + " You are the Winner Congrats! You have " + score1);
                Console.WriteLine(Name.name2 + " Better luck next time. You have " + score2);
                    Console.ReadLine();
                    Console.WriteLine(Name.name + " and ");
                    Console.WriteLine(Name.name2 + " Thanks for playing my game. come back soon you hear?");
                    Console.ReadLine();

            }
            else
            
                Console.WriteLine( Name.name+" and"  );
            Console.WriteLine(Name.name2 + " You both  have the same score, it's a tie!");
            Console.ReadLine();
            Console.WriteLine(Name.name + " and ");
            Console.WriteLine(Name.name2 + " Thanks for playing, come back and try to beat each other the next time, k? ");
            Console.ReadLine();



        }
        }
    }










