import random

# Define a dictionary of user inputs and responses
responses = {
    "hello": ["Hi there!", "Hello!", "Hey!"],
    "how are you": ["I'm good, thanks!", "I'm just a bot, but I'm here to help.", "I'm functioning well."],
    "what's your name": ["I'm a chatbot.", "I don't have a name, but you can call me ChatGPT.", "I go by ChatGPT."],
    "bye": ["Goodbye!", "Farewell!", "See you later!"],
    "default": ["I'm not sure how to respond to that.", "Could you please rephrase that?", "I don't understand."]
}

# Main chatbot loop
while True:
    user_input = input("You: ").lower()

    # Check if the user wants to exit
    if user_input == "bye":
        print("Chatbot: Goodbye!")
        break

    # Search for a response in the dictionary, or provide a default response
    response = responses.get(user_input, responses["default"])
    print("Chatbot:", random.choice(response))
