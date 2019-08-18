# Creating ChatBot

What is a Chatbot?
A chatbot is a piece of software that conducts a conversation via auditory or textual methods. Such programs are often designed to convincingly simulate how a human would behave as a conversational partner, although as of 2019, they are far short of being able to pass the Turing test.

Or simply,chatbot is an artificial intelligence (AI) program that simulates interactive human conversation by using key pre-calculated user phrases and auditory or text-based signals.

# What do I need to know?

Import os, chatterbot. From chatterbot, import ChatBot, ListTrainer, ChatterBotCorpusTrainer, and you're pretty much done.

```markdown
import os 
#import chatterbot
from chatterbot import ChatBot
from chatterbot.trainers import ListTrainer
from chatterbot.trainers import ChatterBotCorpusTrainer
```
![Image](https://pbs.twimg.com/media/DceA9yzWAAAk64X.jpg:large)

# Okay, what next?

Name your bot! I'll name it Candid.

```markdown
bot = ChatBot("Candid")
```

Next off, train it!

```markdown
trainer = ChatterBotCorpusTrainer(bot)

trainer.train(
    "chatterbot.corpus.english"
)

#Train the chatbot based on the english corpus
trainer.train("chatterbot.corpus.english")
```

# Let's start coding!

```markdown
while True:
    message = input("You: ")
    if message.strip().lower() != "bye":
      reply = bot.get_response(message)
      print("Candid: ",reply)
    elif message.strip().lower() =="bye":
      print("Candid: ",GoodBye!)
      break
```

# And, you're done!

Just follow these steps, and congrats! You've created your first chatbot!

For more details see [my account](https://github.com/jsxs0).

# Support or Contact

Having trouble with the code? [Contact me](https://github.com/jsxs0) and I’ll help you sort it out.
