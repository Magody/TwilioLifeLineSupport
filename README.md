*This is a submission for the [Twilio Challenge ](https://dev.to/challenges/twilio)*

## What I Built
In a world where mental health issues are becoming increasingly prevalent, our mission is to offer a safe, supportive, and non-judgmental space for individuals to share their struggles and receive immediate, compassionate guidance.

I would have liked to have had something like this on hand; some years ago.

Harnessing the capabilities of Flask for our web framework, Twilio for seamless voice and SMS communication, and the advanced language models from OpenAI, I have created a tool that listens, understands, and responds with empathy and care.

**Features:**
1. Real-time voice Emotional Support: Users can reach out at any time by **calling** a dedicated number, where they are greeted by a responsive and empathetic voice ready to listen and help.
2. Supportive and Non-judgmental: Every interaction is crafted to be positive and supportive, creating a safe space for users to open up about their feelings.
3. Summarizing Advice: If a user decides to end the conversation, the chatbot provides a summarized advice via **SMS**, ensuring the user has a tangible reminder of the support received.

The system looks like this, I developed a microservice to handle the real time interaction and logic:

![System Architecture](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/d54tgtia93wijz4qsmq3.png)

Inside de service, there is a graph of LLMs collaborating to produce a helpful system:

![Service flow](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hjs3u8tqrfxr0a01ll4y.png)

## Demo

[Code](https://github.com/Magody/TwilioLifeLineSupport/tree/main): https://github.com/Magody/TwilioLifeLineSupport/tree/main

{% embed https://drive.google.com/file/d/18sTIw3wWpvZvecz1zeyJX45Z4bKBcRsa/preview %}

{% embed https://drive.google.com/file/d/1BypmvvApB5jOd4fEONuuZum9oe4jl3xp/preview %}

## Twilio and AI

**Twilio**
A. Voice Communication:

- Voice Calls
- Twilio Voice Response (TwiML): I utilized Twilio’s Voice Response capabilities to handle incoming calls.

B. SMS Communication:

- Sending Summaries: The system uses Twilio to send a summarized SMS containing the key points of the advice provided.
- Follow-Up Messages: Twilio’s SMS service is also used to send follow-up messages, providing additional resources or encouragement as needed.

**AI Integration**

A. Natural Language Processing (NLP):

- Understanding User Input: OpenAI’s language models enable the chatbot to accurately understand and process the user’s spoken words.
- Generating Compassionate Responses: The AI generates responses that are compassionate and empathetic.

B. Context-Aware Conversations:

- Maintaining Continuity: The AI keeps track of the conversation’s context by storing previous interactions in text files. 
- Handling Crisis Situations: The AI can recognize when a user might be in crisis and responds with appropriate, comforting messages, encouraging the user to seek professional help if necessary.

## Additional Prize Categories

I think the projects is in the following categories
- Twilio Times Two: The project uses 2+ Twilio APIs (Call, SMS).
- Impactful Innovators: The project tries to drive positive social impact.

# Features

- Real-time Support: Provides immediate, empathetic responses to users seeking mental health advice or emotional support.
- Compassionate Conversations: Engages in positive, non-judgmental dialogue to foster a safe environment for users to express their feelings.
- Crisis Intervention: Offers supportive messages and encourages seeking professional help for individuals experiencing a crisis.
- Personalized Advice: Delivers tailored advice on stress management, anxiety reduction, sleep improvement, relationship issues, and more.
- Resource Recommendations: Suggests helpful resources and coping strategies to promote mental well-being.

# Technologies Used

- Flask: A lightweight WSGI web application framework for building the server.
- Twilio: For handling voice and SMS communication.
- OpenAI: Advanced language models to generate compassionate and helpful responses.
- Python: Core programming language used for the project's development.
- dotenv: For managing environment variables securely.

# For development

- git clone https://github.com/your-username/lifeline-support.git
- cd lifeline-support
- pip install -r requirements.txt
- Fill your environment variables
- python app.py

# Contributing:

We welcome contributions from the community. If you would like to contribute, please fork the repository and create a pull request with your changes. Make sure to follow the project's code of conduct.

# Contact

For any questions or support, please contact [danny.sebastian.diaz@gmail.com].
