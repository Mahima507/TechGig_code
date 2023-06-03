# TechGig_code

2.Problem The Magic Wand.
You are a wizard who possesses a magical wand that can be used to change the values of an array. Your wand has two powers: Increase and Decrease. With each use of the wand, you can either increase or decrease any element of the array by 1.


One day, a group of villagers came to you with a problem. They had an array of positive integers of size N and a set of queries of size M. For each query, queries[i], they wanted to make all the elements of the array equal to queries[i] using your magic wand.


To help the villagers, you decided to use your magic wand to perform the operations. However, each time you perform an operation, the cost of using your wand increases. The cost of using your wand for an operation on an element is equal to the absolute difference between the value of the element and the desired value after the operation.


Example:

If you want to change an element from 5 to 3, it will cost you 2. If you want to change an element from 7 to 8, it will cost you 1.


You can perform any number of operations on any element of the array for a given query. However, the cost of using the wand for each operation accumulates, and you want to minimize the total cost of all operations for each query.

Input Format
The first line of the input consists of two space-separated integers N (length of array) and M (length of queries).

The second line of input consists of N space-separated integers arr[i].

The third line of input consists of M space-separated integers queries[i].


Constraints
1 <= N <= 10^5

1 <= M <= 10^5

1 <= arr[i] <= 10^9

1 <= queries[i] <= 10^9



Output Format
Print a list of integers of cost of length m, where cost[i] is the minimum cost to make all elements of nums equal to queries[i].


Sample TestCase 1
Input
5 3
1 2 3 4 5
5 2 1
Output
10 7 10
Explanation

Number of array elements, N = 5

Number of Queries,M = 3


For the first query, queries[0] = 5, you can increase the elements at indices 0, 1, 2, and 3 by 4, 3, 2 and 1 respectively. Total cost of operations = 10.


For the second query, queries[1] = 2, you can decrease the elements at indices 2, 3, and 4 by 1, 2, and 3, and increase the element at index 0 by 1. Total cost of operations = 7.


For the third query, queries[2] = 1, you can decrease the elements at indices 4, 3, 2, and 1, by 4, 3, 2 and 1. Total cost of operations = 10



1. Problem Forest Fire 

You are camping in a forest area at night. You are living with the forest officers to experience their challenges and hardships to create a documentary on them. Everything was going well. Suddenly, a fire has broken out in the forest and it is expanding exponentially. There is a lot of chaos and cries of animals. It is going to take alot of time for the backup. Some of the posts in the forest have also caught fire. The officers are trying everything to safeguard the animals but the fire is spreading too fast. Amid such chaos, the petrol tankers of the officers have also caught fire. The fire is unstoppable now and the commanding officer is taking important decisions with his officers.


The officers know the energy levels of all the N animals in the forest at the moment. It is a tough decision for them as they can only save exactly X animals because of the current situation of the transports they have. Since, the animals are pride of the forest, the energy level of the animals are represented with P. All the animals with energy level equal to P or greater than P can board the available transports and they will be moved to a safer place. But since the capacity is for exactly X animals it is going to be tough to figure out.


Officer needs your help to figure out the minimum energy level P such that they can get exactly X animals to transport. If it is not possible to save exactly X animals, then you should respond with -1 so that they can think of some other plan. The officers are busy trying to get control of the fire and are counting on you to figure out the minimum P to save and transport exactly X animals. 



Example:

Number of animals, N = 5

Energy level of N animals = { 1, 3, 2, 4, 5 }

Current available capacity, X = 4


You should choose P = 2, so that exactly 4 animals with energy levels (2, 3, 4 and 5) can be saved as these have energies greater than or equal to P.



Input Format
The first line of input consists of two space-separated integers, N (number of animals) and X (available capacity for animals that can be transported).

The second line of input consists of N space-separated integers, representing the energy of all the animals.



Constraints
1<= N <=10^5

1<= X <=N

1<= arr[i] <=10^12



Arr[i] represents the energy level of the ith animal.




Output Format
Print the minimum energy level P such that exactly X animals can be saved or transported. If it is not possible to save exactly X animals, then print -1.

Sample TestCase 1
Input
5 4
1 3 2 4 5
Output
2
Explanation
As explained in the problem.
