# java-prairie-cqp


### Calculator
Implement a Calculator that allows to calculate two number.


### Library

A Book has a title and some pages.<br/>
A CD has a title and a time.<br/>
A DVD has a kind, a title, an indication of it is in 3D and time.<br/>
There are 4 kind of movie: horror, fun, action, musical.<br/>

The Library has these methods only:
* ArrayList<Book> putBooks(ArrayList<Book> books);
* ArrayList<DVD> putDvds(ArrayList<DVD> dvds);
* ArrayList<CD> putCDs(ArrayList<CD> cds);
* boolean isOpen(int hour);

The Library can storage 3 DVDs only.<br/>
If there are already 3 DVDs and the user want to give more. The library doesn't accept these dvds.<br/>
If there are already some DVDs and the user try to give a book that the library already has. The library doesn't accept these dvds.<br/>

For example:<br/>
The library has 3 DVDs and the user give 4 DVDs. The library doesn't accept it. So the library has 3 DVD.<br/>
The library have 1 DVD like DVD dvd = new DVD("dvd", 120, Movie.HORROR, false) and the user give the same DVD. The library doesn't accept it.<br/>

Implement library and create unit test


### UniqueChar
Implement an algorithm to determine if a string on ascii has all unique characters. Create unit test too<br/>
example:<br/>
* abcdefg => ok
* abcdafg => ko


### Mower
The company X wants to develop an auto­mower for square surfaces.<br/>

The mower can be programmed to go throughout the whole surface.<br/>
Mower's position is represented by coordinates (X,Y) and a characters indicate the orientation according to cardinal notations (N,E,W,S).<br/>
The lawn is divided in grid to simplify navigation.<br/>

For example, the position can be 0,0,N, meaning the mower is in the lower left of the lawn, and oriented to the north.<br/>

To control the mower, we send a simple sequence of characters.<br/>
Possibles characters are L,R,F. L and R turn the mower at 90° on the left or right without moving the mower.<br/>
F means the mower move forward from one space in the direction in which it faces and without changing the orientation.<br/>


If the position after moving is outside the lawn, mower keep it's position. Retains its orientation and go to the next command.<br/>
We assume the position directly to the north of (X,Y) is (X,Y+1).<br/>

To program the mower, we can provide an input file constructed as follows:<br/>
The first line correspond to the coordinate of the upper right corner of the lawn. the bottom left corner is assumed as (0,0).<br/>

The rest of the file can control multiple mowers deployed on the lawn. Each mower has 2 next lines :<br/>

The first line give mower's starting position and orientation as "X Y O". X and Y being the position and O the orientation.<br/>
The second line give instructions to the mower to go throughout the lawn. Instructions are characters without spaces.<br/>

Each mower move sequentially, meaning that the second mower moves only when the first has fully performed its series of instructions.<br/>
When a mower has finished, it give the final position and orientation.<br/>

Example:<br/>
input file<br/>
55<br/>
12N<br/>
LFLFLFLFF<br/>
33E<br/>
FFRFFRFRRF<br/>

result<br/>
13N 51E

Implement mower and create unit test.




