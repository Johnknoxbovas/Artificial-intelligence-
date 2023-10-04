# Simple chatbot in Python

# Define a function to respond to user input
def chatbot_response(user_input):
    if "hello" in user_input:
        return "Hello! How can I assist you?"
    elif "how are you" in user_input:
        return "I'm just a computer program, but I'm here to help. What can I do for you?"
    elif "bye" in user_input:
        return "Goodbye! Feel free to return if you have more questions."
    else:
        return "I'm not sure how to respond to that."

# Main loop for the chatbot
while True:
    user_input = input("You: ")
    response = chatbot_response(user_input)
    print("Chatbot:", response)
