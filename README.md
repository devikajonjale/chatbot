# Chatbot
**This chatbot prioritizes retrieving pre-defined responses based on user input, offering a structured interaction experience.** It is trained on the dataset which contains categories (intents), pattern and responses. We use a special recurrent neural network (LSTM) to classify which category the user’s message belongs to and then we will give a random response from the list of responses.

1] Data & Training:
- Dataset: The core of the system is a dataset containing three key elements:
-  - Intents: Categories representing user queries or topics (e.g., "greetings", "options", "conclusion").
-  - Patterns: Sets of example phrases or sentences users might use to express each intent (e.g., "Hi", "Hello!", "Good morning" for the "greetings" intent).
-  - Responses: Pre-defined responses associated with each intent (e.g., "Hi there! I am Bot." for the "greetings" intent).

2] LSTM for Intent Classification: Unlike traditional retrieval chatbots, this project employs a Long Short-Term Memory (LSTM) network – a type of recurrent neural network (RNN). LSTMs excel at analyzing sequential data like text, allowing the model to learn the relationships between words in user queries and their corresponding intents.
- User Input Processing: The user's message is preprocessed (e.g., tokenization, stemming/lemmatization) before being fed into the LSTM.
- Intent Prediction: The trained LSTM analyzes the user's message and predicts the most likely intent category based on the patterns it has learned.

3] Response Retrieval: Once the intent is identified:
- The system retrieves a random response associated with the predicted intent category.
- This ensures a relevant response is provided even if the user's exact wording doesn't perfectly match a training pattern.

referred: https://data-flair.training/blogs/python-chatbot-project

**Output Example of Chatbot:**

![WhatsApp Image 2024-07-01 at 19 26 48_1957b00d](https://github.com/devikajonjale/chatbot/assets/119109892/4aaf5faf-6567-4aeb-ae6e-7b2634942b77)
