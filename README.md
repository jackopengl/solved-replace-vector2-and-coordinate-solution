Download Link: https://assignmentchef.com/product/solved-replace-vector2-and-coordinate-solution
<br>
<p class="ui header product-top-header" title="Replace Vector2 and Coordinate solved"> 1) Replace Vector2 and Coordinate

a) Create a new Vec2 class as a replacement for both Vector2 and

Coordinate. Vec2 must be a templated class, so that it stores and

manipulates X and Y values of a templated type. It may be helpful to

start with the Vector2 class, add “template&lt;typename TYPE” to the

header, and replace (Ctrl+H) each instance of “float” with “TYPE”, and

“Vector2” with “Vec2”.

b) Remember, a templated class must have all method definitions in the

same file as the templated class declaration. Also remember that method

definitions outside of a templated class’ declaration need a

“template&lt;typename TYPE” header, and a “&lt;TYPE” appended to the class

name with the scope resolution operator (e.g.:

“void Vec2&lt;TYPE::limitMagnitude(TYPE max) {/* method body */}”).

c) Replace the use of Vector2 with Vec2&lt;float.

d) Replace the use of Coordinate with Vec2&lt;int.

2) More Game Goals

a) Instead of having a single goal for the player, create at least 3

randomly placed goals for the player. Use a “std::vector&lt;Entity”

object (from the Standard Template Library) named “goals” to store the

goals.

c) Whenever the user clicks in the game window, the game should create

another goal object for the player to get, and add it to the

“std::vector&lt;Entity goals” object.

d) Each retrieved goal should be removed from the game after being

retrieved by the player. A “You Win!” message should display when the

player retrieves all goals.

[Autonomous Agent] The player controlled Entity can move to collect each

goal without any user input!

[He’s Coming, RUN!] Create a MovingTarget class that extends Entity, and use

that for the game goals. Each MovingTarget should wander randomly and

slowly, running away from the player if the player comes withing a

certain radius. Be sure to prevent goal entities from escaping the game

boundaries!

[I’ll Make My Own List] Create your own templated list type and use it

instead of the std::vector class.

[Blocked!] Implement collision detection, so that Entity objects can’t

occupy the same area.

[We’ve Had Enough!] Create a Hunter class that extends Entity, and slowly

follows the player’s Entity, ending the game in defeat if the player

should be caught by a Hunter.

[Let’s Fight!] Create a Projectile class that acts as a projectile attack

for the player’s Entity. Keep track of all projectiles in the game with

a “vector&lt;Projectile” object. If there are Hunters in the game,

give Hunters a projectile attack as well! Don’t forget to remove

projectiles from the game once they hit something or leave the game

boundaries!