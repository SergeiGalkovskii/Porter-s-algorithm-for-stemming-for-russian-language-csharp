##Algorithm Stemmer Porter for Russian language in C#
Stemming algorithm for Russian language. Algorithm find a stem of a word with prefix and return transform word. Algorithn doesn't using dictionaries. It work via rules finded Martin Porter. For details information visit M.Porter's [site](http://snowball.tartarus.org/algorithms/russian/stemmer.html) 

##Алгоритм Стеммер Портера для русского языка на C#.
Алгоритм находит основу слова и возвращает освнову слова с приставкой. Алгоритм не использует словарей, а работает последовательно отсекая окончания и суффиксы. Для более детального ознакомления с алгоритмов посетите [сайт](http://snowball.tartarus.org/algorithms/russian/stemmer.html) Мартина Портера. Алгоритм переписан с PHP версии на C# использую этот [код](http://forum.dklab.ru/php/advises/HeuristicWithoutTheDictionaryExtractionOfARootFromRussianWord.html)

```
using System;

namespace ConsoleApplication
{
    public class Program
    {
        public static void Main(string[] args)
        {
            Console.WriteLine(Porter.TransformingWord("улыбнулся"));
        }
    }
}

```
