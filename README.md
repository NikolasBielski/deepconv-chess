## Chess Data for Deep Learning

Welcome!  This project has two primary goals.  

1.  To teach an agent chess using as little hand-coded knowledge as possible using Keras and TensorFlow.  
2.  To create a community resource of preprocessed chess game data.

As I was researching and preparing to work on the first problem, I noticed that prepared chess game data for machine learning was largely unavailable in large quantities.  It is my hope that this project can contribute to computational chess and deep learning communities by making it easier to access prepared data for machine learning applications.  While the chess engine component will be stored here on GitHub,  the most up to date version of the data sets will be [hosted on data.world](https://data.world/mrklees/deep-convolutional-chess). 

In the data folder you will find a small dataset to get you started.  It is a numpy save files (.npz) including thousands of games which have been processed into numpy arrays. The board states are composed of 6 x 8 x 8 numpy arrays with 6 channels corresponding to the 6 different types of pieces. Each board also corresponds to a numpy array containing the player who is moving and what the next move was including an index corresponding the piece, and the row and column coordinate values. 

The code for this script is largely be developed in Jupyter Notebooks.  As previously mentioned, we are relying heavily on the Keras library for modeling.  The chess-programming python library has also been an extremely valuable resource in handling some of the boring data processing stuff.  As you might expect, we also make heavy use of the numpy library.  As we develop towards a central  Some of the scripts will be extract and formated for .py files as well.

In the course of doing research for this project, I made use of several resources and papers which I list below. They reflect what I think are some of the most exciting approaches in the application of deep learning to chess, and I have learned a ton from them. Giraffe, for example, applies reinforcement learning and deep learning to the problem of chess, and currently ranks 186th on the CCRL chess engine ranking for all engines. If you have ideas, head over to data.world and contribute to the discussion in the data or model talk thread! If you identify concrete problems or suggestions, raise an issue here on GitHub!

#### Built on the Shoulder of Giants
In working on this project I spent a considerable amount of time reading the magnificent content on [the chess programming wiki](https://chessprogramming.wikispaces.com/)

There are also several papers which I leaned on considerably in learning how to create this engine.

*  Oshri, Barak, and Nishith Khandwala. ["Predicting moves in chess using convolutional neural networks."](http://cs231n.stanford.edu/reports/2015/pdfs/ConvChess.pdf) (2016). 
*  Lai, Matthew. ["Giraffe: Using deep reinforcement learning to play chess."](https://arxiv.org/abs/1509.01549) arXiv preprint arXiv:1509.01549 (2015).

Finally, much gratitude to the folks at [KingBase](kingbase-chess.net). KingBase provides 1.9 million games of players > 2000 ELO in multiple formats including pgn.