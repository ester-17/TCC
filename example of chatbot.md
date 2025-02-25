responses = {
    "greeting": ["Hello!", "Hi there!", "Greetings!"],
    "farewell": ["Goodbye!", "See you later!", "Take care!"],
    "help": ["How can I assist you?", "What do you need help with?"]
}

def get_response(user_input):
    for key in responses:
        if key in user_input.lower():
            return random.choice(responses[key])
    return "I'm not sure how to respond to that."

user_input = input("You: ")
print("Bot:", get_response(user_input))
