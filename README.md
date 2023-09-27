# monty_hall_assignment
First assignment for Applied python class. The assignment required that we simulate the switch door strategy of the Monty hall game in python

### Requirements

- You are on a TV show and there are three doors in front of you: Two of them with a goat behind and one with a car;

- The host knows where the car is;

- I want you to simulate that you are a contestant on this show 1000 times. Each time, you pick a random door as your first choice, let the host open a door that reveals a goat, and then switch your choice to the door that the host didn't open. With that strategy (known as the "always switch" strategy), how often do you win the car? Show me the percentage!


Here are a couple of details that I want to be clear:
- Before starting each game, the host randomly selects which door contains the car.

- After you make your initial choice, the host always opens one door that contains a goat, and it will always be a door that you did not initially choose. (If the host has two options for which door to open to reveal a goat, he will randomly select which of those two doors to open.)

- After the host opens a door that contains a goat, you will always be given the option to switch your choice to the door that is still closed, and you will always accept that option.




### Algorithm ( solution outlined)
1. there are three doors; 2 have goats, 1 has a car (a list with 3 index, a car could randomly be behind one)
2. Contestant picks a random door (first choice)
3. The host opens another door that has a goat
4. Switch choice to the door that hasn't been opened (switch strategy)
5. Show number of times you win the car
6. Show a percentage


#### Execution
1. Create a function 'monty_game'
2. The function accepts two parameters, first the chances (i.e the number of times the player gets to play), then the switch strategy, which is True
3. the three doors are represented by a list with three 0's, representing 'goats'
4. randomly replace one of the doors with the a car
5. set the car to the door index 1
6. contestant makes a random choice
7. monty chooses a door which has a goat
8. the contestant, based on the switch strategy will opt for the door which has not been opened
9. count the number of cars the player potentially makes with each iteration
10. calculate the percentage

Keywords:

.choice() module - returns a randomly selected element from a specified sequence


.next() - the next function returns the next item in an iteration

the f-string provides a concise way to concatenate strings, and at the same time embed integer values by enclosing them in curly brackets.

Results:
the game runs a 1000 times and prints the percentage of the wins if the player employs the switch strategy
