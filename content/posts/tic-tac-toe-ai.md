---
title: "Tic Tac Toe Ai"
date: 2023-06-08T14:32:07+02:00
draft: true
---

Recently I got interested in machine-learning and made some basic algorithms like svm etc. and I didn't really know what to do with it.
Then I thought of tic-tac-toe and immediately knew what I wanted to do: write a tic-tac-toe-ai!

Althouth minimax isn't machine-learning, the definition for AI is really vague so I just call it that.

## How it works

The algorithm is called minimax. It's really simple.
To find the best move, you basically just have to assume the opponent always plays the best moves.

To evaluate a given move, you follow simple steps:

- If a player has won, return the player (-1 or 1)
- For every possible move, evaluate each and return the best move for the player whose turn it is

As you can see, this is a recursive algorithm which is part why I like it.

Since the players alternate turns, the algorithm alternately chooses the minimum and maximum evaluation. Thats why it's called minimax.

You can also add a depth limitation or such things but this is optional.

## Building it

The first thing you need for a tic-tac-toe-ai is tic-tac-toe.
I just made a simple 2-player game as a cli. No fancy gui.

Then I added an evaluation which first didn't work that well but I managed to fix it.

At last I just removed the second player and just let the game automatically play the best move which it finds by choosing the move with the best evaluation.

I just polished the UI a little bit and was finished. I managed doing it all in an afternoon. It was really simple.

## Conclusion

This was really fun, I highly recommend also doing it.

You can find the whole project on [github](https://github.com/AinoSpring/tic-tac-toe-ai).

