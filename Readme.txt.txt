Covid-19 Tracker application provides the details of covid-19 cases in USA or a specific state in USA to user mobile phone.
The application fetches the data from covid tracking api(https://covidtracking.com/api/).

Dependencies:
1. Python3
2. Flask
3. Ngrok
4. Twilio Messaging Service.

Working Procedure:
1. User sends a message to Twilio number(Message:"What's the status in US?")
2. Twilio Sends the POST request to the Flask application through ngrok service and Twilio message webhooks.
   - Flask application is made public through ngrok service.
3. Flask application fetches the data from api and sends back the response in Twilio Markup Language.
4. Twilio service sends the output back to the user which is received from the flask application. 
