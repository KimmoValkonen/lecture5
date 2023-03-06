# Activities

## Task 1

- Refer to the following link. Discuss how the
  Recursive Factorial works:
  https://www.cs.usfca.edu/~galles/visualization/RecFact.html
- Refer to the following link. Discuss how the Recursive Fibonacci works:
  https://www.cs.usfca.edu/~galles/visualization/DPFib.html
# : Keskustelimme aiheista

## Task 2

There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs at a time. There is a simple implementations in `./src/` folder. Discuss how the code works.
# : Tämä koodi on kirjoitettu C++-kielellä, ja se laskee niiden polkujen määrän, joita voidaan kulkea n askeleen pituisen matkan kulkemiseen.

Funktio number_of_paths(int n) ottaa syötteenä kokonaisluvun 'n' ja palauttaa kokonaisluvun, joka kuvaa mahdollisten polkujen lukumäärää, jolla voidaan kulkea 'n' askelta.

Funktio käyttää aluksi kolmea perustapausta käsitelläkseen skenaariota, jossa syöttöarvo on 0, 1 tai 2. Jos syöttöarvo on 0, se tarkoittaa, että 0 askeleen kattamiseen ei ole mitään polkua, joten se palauttaa 0. Jos syöttöarvo on 1, yhden askeleen kattamiseen on vain yksi tapa, joten se palauttaa 1. Jos syöttöarvo on 1, se palauttaa 1. Vastaavasti, jos syöttöarvo on 2, on kaksi tapaa kattaa 2 askelta, joten se palauttaa 2.

Jos syöttöarvo on suurempi kuin 2, funktio kutsuu itseään rekursiivisesti kahdesti vähentämällä 1 ja 2 syöttöarvosta 'n'. Näiden kahden rekursiivisen kutsun tulos lasketaan yhteen, jolloin saadaan funktion lopullinen tulos.

Pääfunktiossa number_of_paths(4)-funktiokutsun palauttama arvo tulostetaan konsoliin cout-lausekkeella, joka on "number of paths = 5", koska on olemassa viisi mahdollista polkua, jotka kattavat neljä askelta. 

## Task 3

- There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs or **3 stairs** at a time. Write a program that counts the number of ways, the person can reach the top. You can use the following program as a starter `./src/staircase1.cpp`. Also the link below might useful:
  https://www.includehelp.com/cpp-programs/stair-case-program-to-solve-the-staircase-problem.aspx

# Vastaus:
#include <iostream>
using namespace std;

int number_of_paths(int n)
{
    if (n <= 0)
        return 0;
    if (n == 1)
        return 1;
    if (n == 2)
        return 2;
    if (n == 3)
        return 4;

    return number_of_paths(n - 1) + number_of_paths(n - 2) + number_of_paths(n - 3);
}

int main()
{
    int n;
    cout << "Enter the number of stairs: ";
    cin >> n;
    cout << "number of paths =  " << number_of_paths(n);
    return 0;
}

## Task 4: Individual (at home)

- What are the pros/cons of recursive over iterative Programming?
  # Vastaus: 
  + Se on helpompi kirjoittaa ja ymmärtää
  - Voi hävitä suorituskyvyssä

- Difference between recursion and induction.
1.	Recursion is the process in which a function is called again and again until some base condition is met. 	Induction is the way of proving a mathematical statement. 
2.	Recursion is the way of defining in a repetitive manner.	Induction is the way of proving.
3.	Recursion starts from nth term till the base case. 	Induction starts from the initial till (n+1)th term. 
4.	
Recursion has two components:
Base condition
Recursive step.

Induction has two steps:
Base step
Inductive step
5.	Recursion: We backtrack at each step to replace the previous values with the answers using the function.
Induction: We just prove that the statement is true for n=1. Then we assume that n = k is true. Then we prove for n=k+1.
6.	Recursion: No assumptions are made. 	Induction: The assumption is made for n= k
7.	Recursive function is always called to find successive terms. 	Induction: Here statements or theorems are proved and no terms are found. 
8.	Recursive function can lead to infinity if no base condition is given. 	Induction: There is no concept of infinity. 

> Refer to the [links](#links) section below.

## Links

- https://cpp.sh/
- [Difference Between Recursion and Induction](https://www.geeksforgeeks.org/difference-between-recursion-and-induction/)
- [Recursion vs Iterative Programming](https://www.softwaretestinghelp.com/recursion-in-cpp/)
