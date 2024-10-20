import random

class RockPaperScissors:

    def _init_(self, player1, player2='Computer'):
        """Constructor to initialize the players"""
        self.player1 = player1
        self.player2 = player2
        self.moves = ['rock', 'paper', 'scissors']

        def get_move(self, player):
        # """Method Overloading: Get move for the player or computer"""
            if player == 'Computer':
                return random.choice(self.moves)  
            else:
                while True:
                    move = input(f"{player}, enter your move (rock, paper, scissors) or 'quit' to exit: ").lower()
                    if move in self.moves or move == 'quit':
                        return move
                    else:
                        print("Invalid move. Please try again.")

    def determine_winner(self, move1, move2):
        """Method to determine who won the round"""
        print(f"{self.player1} chose {move1}, {self.player2} chose {move2}")
        if move1 == move2:
            print("It's a tie!")
        elif (move1 == 'rock' and move2 == 'scissors') or \
             (move1 == 'scissors' and move2 == 'paper') or \
             (move1 == 'paper' and move2 == 'rock'):
            print(f"{self.player1} wins this round!")
        else:
            print(f"{self.player2} wins this round!")
    
    def play_game(self):
        """Method to play the game in a loop until the user decides to quit"""
        while True:
            print("\n--- New Round ---")
            player1_move = self.get_move(self.player1)
            if player1_move == 'quit':
                print("Thanks for playing!")
                break
            
            player2_move = self.get_move(self.player2)
            if player2_move == 'quit':
                print("Thanks for playing!")
                break
            self.determine_winner(player1_move, player2_move)
    
if _name_ == "_main_":
    player_name = input("Enter your name: ")
    game = RockPaperScissors(player1=player_name) 
    game.play_game()
