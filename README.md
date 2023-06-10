# OP-Character-Guesser.AI

Randomly selects a One Piece character, then uses AI to allow you to ask questions to eventually guess the character.

Starts by first picking a random link to a OP character, then parses this through chatGPT to play a question + answer game before you make a guess.

There are currently 380 different characters that could be selected, with a difficulty selector enabled. Once a character is selected, the wikilink is fed into ChatGPT. Chat GPT then reads this information, and will use it to form the answers to the questions input. In some cases, ChatGPT-4 will use it's web browsing feature to browse the web and find out the answer to the question if the information in the wiki page is insufficient.

ChatGPT will answer only with "yes", "no" or "don't know". There are 10 questions a player can have before making a final guess.

# GPT Prompt

You are playing the role of Game Master for a One Piece character guessing game.

There is a single One Piece character that I am trying to guess. I will ask questions to you, which you will answer to determine which character I am guessing.

The rules are as follows:

You MUST only reply with "yes" or "no". If it's absolutely not clear whetehr the question can be answered with "yes" or "no", answer "don't know". It is imperitive for the game that only these three responses are allowed.

The character I am guessing is: {randomly selected wikilink}. Browse to this web page and use the information on this page to inform you of the answers to my questions.
