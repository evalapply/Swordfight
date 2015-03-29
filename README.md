# Swordfight

"*A game of chess is like a sword fight. You must think first before you move.*" (Shaolin vs Wutang)

This is going to be a chess engine. No GUI, just a chess AI.

It's for fun. I know Clojure is not a good choice for a chess engine.

## Usage

1. Download this repo.
2. Install [Leiningen](http://leiningen.org/) (requires Java JDK version 6 or
   later).
3. Install [XBoard](https://www.gnu.org/software/xboard/) (should be available
   in your favorite package manager).
4. Run `xboard` and choose `Engine -> Load New 1st Engine`.
   To add Swordfight as a new engine you need to point to the repo directory
   and set `lein run` as command. This will make Swordfight play as black.
5. Play your first move.
6. Swordfight plays a Mexican Defense (a.k.a. Kevitz–Trajkovic Defense a.k.a. Black Knights' Tango)
   and resigns after your third move. If you run `xboard -debug` there will be some debugging info
   in the `xboard.debug` file.

That's it for now...

## Protocol

This engine will slowly become more and more
[CECP](https://en.wikipedia.org/wiki/Chess_Engine_Communication_Protocol)-compatible.
Basically what it means is it reads from standard input and writes to standard output
following a commonly used protocol, which is based on GNU Chess CLI and designed by
Tim Mann, the author of XBoard. It's quite possible that Swordfight will support
Universal Chess Interface or other protocols in the future.

## Did you know?

The field of computer chess started with
[*Programming a Computer for Playing Chess*](http://archive.computerhistory.org/projects/chess/related_materials/text/2-0%20and%202-1.Programming_a_computer_for_playing_chess.shannon/2-0%20and%202-1.Programming_a_computer_for_playing_chess.shannon.062303002.pdf),
a 1950 paper by [Claude Shannon](http://en.wikipedia.org/wiki/Claude_Shannon). Why is it that old papers are better than new ones? I don't know.

Did you know that the number of possible positions in chess is bigger than the number of atoms in the observable universe? That's a lot of positions!

I think unicode chess pieces look pretty neat!

♜ ♖ ♞ ♘ ♝ ♗ ♛ ♕ ♚ ♔ ♟ ♙

Depending on the terminal the colors may be confusing. ♜ is black.

## License

Distributed under the 2-clause BSD license.
