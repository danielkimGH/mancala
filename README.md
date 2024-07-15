# mancala
Text based version for Mancala game. Click [HERE](https://www.scholastic.com/content/dam/teachers/blogs/alycia-zimmerman/migrated-files/mancala_rules.pdf) to learn how to play!

**Mancala:** The Mancala object represents the game as played. Contains information about the players and game board
- **create_player:** Takes one parameter of the player’s name as a string and returns the player object
- **print_board:** Prints board information
- **play_game:** Takes two integer parameters of player number and pit index

**Simulation Example (input)**

      game = Mancala()
      player1 = game.create_player("Lily")
      player2 = game.create_player("Lucy")
      print(game.play_game(1, 3))
      game.play_game(1, 1)
      game.play_game(2, 3)
      game.play_game(2, 4)
      game.play_game(1, 2)
      game.play_game(2, 2)
      game.play_game(1, 1) # special rule of opposite sum occurs
      game.print_board()
      print(game.return_winner())

**Simulation Example (output)**

      player 1 take another turn
      [4, 4, 0, 5, 5, 5, 1, 4, 4, 4, 4, 4, 4, 0]
      player 2 take another turn
      player1:
      store: 10
      [0, 0, 2, 7, 7, 6]
      player2:
      store: 2
      [5, 0, 1, 1, 0, 7]
      Game has not ended
