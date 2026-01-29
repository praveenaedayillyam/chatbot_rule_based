# Rule-Based Chatbot
## Introduction
- This is a simple rule-based chatbot that provides responses to predefined questions stored in a JSON file. If a user asks a question that is not present in the JSON file, the chatbot will return an inaccurate or default response.  <br><br>
- JSON File Structure <br><br>
The chatbot operates based on a JSON file containing three key elements:<br>
●	Tag: A category or identifier for a specific group of questions.<br>
●	Pattern: A list of questions or variations that users might ask.<br>
●	Responses: Predefined replies that the chatbot can provide when a matching pattern is found.<br><br>
- Example JSON Structure:<br><br>
{<br>
    "intents": [<br>
        {<br>
            "tag": "greeting",<br>
            "patterns": ["Hello", "Hi", "Hey"],<br>
            "responses": ["Hello! How can I assist you?", "Hi there! What can I do for you?"]<br>
        },<br>
        {<br>
            "tag": "goodbye",<br>
            "patterns": ["Bye", "See you", "Goodbye"],<br>
            "responses": ["Goodbye! Have a great day!", "See you soon!"] <br>
        }<br>
    ] <br>
} <br>

- How It Works <br><br>
1.	User Input: The chatbot receives input from the user.<br>
2.	Pattern Matching: It compares the input with the patterns stored in the JSON file.<br>
3.	Response Selection: If a match is found, the chatbot provides a response from the corresponding list.
4.	Default Response: If no match is found, the chatbot returns a generic response such as "I'm sorry, I don't understand that question.
