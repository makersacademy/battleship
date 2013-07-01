# Battleship Challenge

*Aim:* Design [Battleship Game](https://en.wikipedia.org/wiki/Battleship_(game)) in ruby.

### Description of game
 * Follows simple [rules](http://boardgames.about.com/od/battleship/a/Rules-of-Battleship.htm) with the aim of sinking an opponents ship.
 * There are two players.
 * Each player has a 10x10 grid, with cells A1 through J10
 * There are different sizes of ships which can be placed on the grid in the preparation stage of the game. 
 * Each round, players take turn to guess where to launch an attack, aiming to hit their opponents ship.

### Things to do
 * Implement the game!
 * Design system for user input
 * Think about how to keep track of hits and misses.
 * Unit tests. Integration tests.

### Design considerations
 * Another developer should be able to use your code without needed to make significant changes to your classes. Classes should be [open](http://en.wikipedia.org/wiki/Open/closed_principle) to another developer extending their use.
 * Don't have to worry about display? Flexible enough that we have to do little more than [rename methods](http://stackoverflow.com/questions/4763121/should-i-use-alias-or-alias-method) to get it to work with our display?
 * Structure of the code- if designed well then classes will not depend heavily on each other. If designed badly then the tests will have to be long integration tests instead of small unit tests.

### Advance design considerations
 * Game state objects not tied directly to the way you are thinking of displaying it. Another developer might choose to display the game in terminal, on a web page, or as a web service accessed on a phone.
 * Code not directly tied to the input, so it is possible for another developer to add alternate input forms. Keyboard, mouse, gamepad, AI, website?
 * Keeping the [game logic](http://en.wikipedia.org/wiki/Business_logic) separate, so small variants to the rules could be added without having to change much of the other code and tests.

### James own aims
 * Create potential for changing requirements somewhere, to encourage flexibility
 * Ensure that if there are any over complicated or time consuming parts, there is a black box gem/module which they can use to simplify the task.
 * Encourage thinking about code structure, and avoiding tight coupling. Ideally design the task so thinking about this happens as a side effect without directing students to think about it.
