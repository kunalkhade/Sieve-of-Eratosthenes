## Sieve-of-Eratosthenes
Implementation of Sieve of Eratosthenes is an ancient algorithm using openMp (Parallel Programming) 

## Program Description
In mathematics, the Sieve of Eratosthenes is an ancient algorithm for finding
all prime numbers up to any given limit. It uses iterative marking as composite (i.e., not prime) the multiples of each prime, starting with the first prime number, 2. The multiples of a given prime
are generated as a sequence of numbers starting from that prime, with constant difference between them that is equal to that prime. This is the sieve’s key distinction from using trial division to sequentially test each candidate number
for divisibility by each prime.

Shared Element : limit \\
Private Element : i \\
Thread Count : 8 \\

## Compilation process 
1 . gcc -g -Wall -fopenmp -o se SieveEratosthenes.c -lm

2 . ./se Value (number of iterations)

## Result 
Complete code run successfully till 1000 values but over the thousand
it create problem in multi threading

Dynamic Scheduling : 0.0534 millisecond (1000 iteration)

Static Scheduling : 0.0135 millisecond (1000 iteration)

