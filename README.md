##Porter's algorithm for stemming for Russian language in C#
Stemming algorithm for Russian language. Algorithm find a stem of a word with prefix and return transform word. Algorithn doesn't using dictionaries. It work via rules found Martin Porter. For details information about algorithm visit M.Porter's [site](http://snowball.tartarus.org/algorithms/russian/stemmer.html). Algorithm was migrating from PHP [version](http://forum.dklab.ru/php/advises/HeuristicWithoutTheDictionaryExtractionOfARootFromRussianWord.html).

##Алгоритм Стеммер Портера для русского языка на C#.
Алгоритм находит основу слова и возвращает освнову слова с приставкой. Алгоритм не использует словарей, а работает последовательно отсекая окончания и суффиксы. Для более детального ознакомления с алгоритмов посетите [сайт](http://snowball.tartarus.org/algorithms/russian/stemmer.html) Мартина Портера. Алгоритм переписан с PHP версии на C# использую этот [код](http://forum.dklab.ru/php/advises/HeuristicWithoutTheDictionaryExtractionOfARootFromRussianWord.html)

```cs
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
