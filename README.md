# BasesCutter
This script does the following:
1. Loads all games from two .pgn files.
2. For each game in the first file, it finds the game with the highest number of identical moves in the second file.
3. From these identical moves, it creates a new game.
4. Saves the created games in a third .pgn file.
That program was created by ChatGPT-4 few hours ago, I already have that script and it works without errors.
What's so genius about it?
The genius is that if the first database contains 1-0 games and the second database contains drawn games, IN THE THIRD DATABASE (created by the script in the way I described) THERE ARE GAMES IN WHICH THE LAST MOVE IS EITHER BLACK OR WHITE.
If the last move in the third database is WHITE, then the following can be logically concluded:
- there are at least two subsequent BLACK moves, one in the first database with 1-0 games and the other in the second database with drawn games. So, in that line, THERE IS A BLACK MOVE that guarantees a draw for Black!
- if the last move in the third database is BLACK, it means that in the first database with 1-0 games THERE IS A WHITE MOVE after which there is no black move leading to a draw!
Then, everything is checked in the same logic in case the first database has 0-1 games and the second one contains drawn games.
Of course, in the second database, there don't have to be only drawn games, but also wins for the opposite color, but the logical reasoning there is more difficult and maybe another time about those cases.
Which program do I and ChatGPT-4 need to create now? A program that separates games from the THIRD DATABASE into games where the last move was played by Black and games where the last move was played by White. That's the, in my opinion, easier program that ChatGPT-4 needs to create.
