# Minesweeper Game in C++ #

This code implements a minesweeper game in shell and also in a graphical user interface ***wxWidgets***.

## Prerequisites ##

Before running this code, ensure you have the following :

- ***g++*** compiler installed on your system.
- ***wxWidgets*** installed on your system.

Sur ***Ubuntu*** :
```bash
sudo apt-get install libwxgtk3.0-dev
```

## Usage ##

1. Navigate to the **Code** directory containing the source code and the ***Makefile*** file.
```bash
cd Code
```
2. Compile the minesweeper game on both shell and graphical user interface by running ***make all***. Run ***make shellGame*** to just compile the minesweeper on shell. Run ***make wxGame*** to just compile the minesweeper on graphical user interface.
```bash
make all
```
```bash
make shellGame
```
```bash
make wxGame
```
3. The compiled program(s) ***shellGame*** or/and ***wxGame*** is/are now located in the parent repository.
```bash
cd ..
```
4. Execute the compiled game on shell by running ***./shellGame***. Execute the compiled game on graphical user interface by running ***./wxGame***.
```bash
./shellGame
```
```bash
./wxGame
```

*(Optional)* 5. Clean the repository by running ***make clean*** in the **Code** directory.

```bash
cd Code
make clean
```

## Monitor ##

### ShellGame ###

To configure parameters for the minesweeper game in shell, the user have to inform some piece of information. In chronological order, the user have to provide :
- ***Height*** : Integer value which indicates the height of the minesweeper game.
- ***Width**** : Integer value which indicates the width of the minesweeper game.
- ***Total number of mines*** : Integer value which indicates the total number of mines.

Then, the user enter in iterative monitor until the end of the game.

During the iterative monitor, the user have to iteratively insert :
- ***Height*** : Integer value which indicates the height coordinate of the case.
- ***Width**** : Integer value which indicates the width coordinate of the case.
- ***Action*** : Boolean 0 or 1 to respectively indicate whether this action is to discover the case or flag it.

The end of the game comes either with a victory condition, a failure condition or by insert the value ***Exit***, at any moment in the iterative monitor, to exit the game.

### wxGame ###

## To do list ##

- [ ] Add a IA tool to iteratively solve the minesweepper. More especially for the graphical user interface version.
- [ ] Explain the victory condition and failure condition in the usage README file.

### shellGame ###

- [ ] Test the well functioning of the program shellGame :
    - [ ] Height, Width and TotalNumberOfMines : Test the bounds of valid values.
    - [ ] Height, Width and Choice : Test the bounds of valid values.
    - [ ] Test conditions of victory or failure.
- [ ] Edit iterative monitor to include the choice mine or flag when the user insert coordinates.
- [ ] Translate monitor of shellGame in english.

### wxGame ###

- [ ] Add a description monitor game in the README file.
- [ ] Check if there is not an error when the user select a box and the program scan the wrong case. Especially when the minesweeper is not squared.
