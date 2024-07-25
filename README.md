# <p align="center"> Javascript X-chatbot plugin example </p>

<p> Itegrated Chat GPT and General Machine learning model </p>

<p>
<b>How to run application in localhost </b>

You can run your file in http-server.

1> Have Node.js installed in your system.

2> In CMD, run the command npm install http-server -g

3> Navigate to the specific path of your file folder in CMD and run the command http-server

4> Go to your browser and type localhost:8080. Your Application should run

</p>

<p>Main feature of X-AI bot plugin is you can cutomize according to specific domains</p>
<p>For example, if it’s for healthcare, specify the topics like insurance claims, medical appointments, etc.</p>
<p>X-Bot integrated with NLP techniques to understand and process user queries and uses spaCy, NLTK and pre-trained model BERT</p>
<p>It has capabilities of filtering mechanism to restrict responses to domain-specific queries. If a query falls outside the domain, X-chatbot can respond with a cutomizable message like, “I’m sorry, I can only assist with healthcare-related questions. X-Bot is Continuously train and customize based on user interactions to improve accuracy and relevance.</p>

<b>Sample Code:</b>
```python
def is_domain_specific(query):
    # Define keywords related to your domain
    domain_keywords = ["appointment", "insurance", "claim", "doctor", "health"]
    return any(keyword in query.lower() for keyword in domain_keywords)

def chatbot_response(query):
    if is_domain_specific(query):
        # Provide domain-specific response
        return "Here's the information you requested about healthcare."
    else:
        # Provide a generic response for out-of-domain queries
        return "I'm sorry, I can only assist with healthcare-related questions."

# Example usage
user_query = "I want to be a billionaire"
response = chatbot_response(user_query)
print(response)


![Alt text](./images/pic.gif?raw=true "Title")



