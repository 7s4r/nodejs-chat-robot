# nodejs-chatbot
A robot who can talk with you and answer to all questions using OpenAI

```
curl https://api.openai.com/v1/engines/davinci/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -d '{
  "prompt": "The following is a conversation with an AI assistant. The assistant is helpful, creative, clever, and very friendly.\n\nHuman: Hello, who are you?\nAI: I am an AI created by OpenAI. How can I help you today?\nHuman: I'd like to cancel my subscription.\nAI:",
  "temperature": 0.9,
  "max_tokens": 150,
  "top_p": 1,
  "frequency_penalty": 0.0,
  "presence_penalty": 0.6,
  "stop": ["\n", " Human:", " AI:"]
}'
```
