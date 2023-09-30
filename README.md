CHATBOT DEPLOYMENT WITH IBM CLOUD WATSON ASSISTANT

Kevin Harris     (au110121104308)
Abdul Salam      (au110121104004)
Abubukar Siddiq  (au110121104005)
Jagan            (au110121104307)
Surya Prakash    (au110121104320)
Sharukhan        (au110121104318)

PROBLEM DEFINITON 
1.	Goal: Use IBM Cloud Watson Assistant to deploy a fully working chatbot that can comprehend and reply to customer inquiries, giving correct information and improving user experience on a digital platform.
2.	Background: Chatbots have evolved into a crucial tool for improving user experience on digital platforms, thanks to the quick development of artificial intelligence. Utilizing IBM Cloud Watson Assistant's powerful platform for creating, training, and deploying chatbots is essential for providing users with high-quality service.
3.   Important Requirements :
a. Data Security: Ensure that all user data and communications with the chatbot are handled securely and in accordance with applicable data protection laws.
b. Custom Training: Train the chatbot using data that is pertinent to the industry, making sure it is aware of the particular subtleties and jargon used there.  
c. Integration: Ensure minimal downtime and a seamless user experience by seamlessly integrating the chatbot with the digital platform (such as a website or mobile app).  
d. Monitoring & Feedback Loop: Create a system to track the chatbot's performance and take user comments into account to increase its efficacy and accuracy.  
e. Scalability: As the platform expands, make sure the chatbot solution can handle an increasing volume of user enquiries.
4.   Restrictions: 
a. amount: A little amount has been set out for the deployment and upkeep of the chatbot.  
b. Timing: To support an impending marketing campaign or event, the chatbot must be implemented quickly.  
c. Technical: Potential barriers to connecting the Watson Assistant with current IT systems or outside software.
5.   Expected Results:  
A useful chatbot  with over 90% accuracy in understanding and responding to user inquiries.  
b. A substantial decrease in manual customer service efforts as a result of the automation of frequent enquiries.  
c. Increased user engagement and satisfaction with the digital platform.
6.   Evaluation Criteria: 
a. User Satisfaction Rate: The proportion of users who were pleased with the chatbot's responses.  
The average amount of time it takes the chatbot to answer to a user enquiry.  
c. Resolution Rate: The percentage of inquiries that the chatbot effectively answers without requiring human assistance.  
d. Error Rate: The proportion of queries for which the chatbot gave incorrect or unnecessary answers.
7.   Future Aims:
a. Expand the chatbot's language support capabilities in order to serve a global user base.  
b. Integration with other IBM Cloud AI services for a more customized user experience, such as sentiment analysis.  
c. Ongoing development and update of the chatbot's knowledge base to keep up with developments in the market.
DESIGN THINKING
Integrating Chatbot with Facebook Messenger:
1.	Facebook Page and App:
•	Create a Facebook Page for your chatbot/service.
•	Create a new App at Facebook Developers Portal.
2.	Set up Messenger:
•	In the App’s dashboard, under “Add a Product”, select “Messenger”.
•	Generate a Page Access Token by selecting your page. Save this token; you’ll need it to set up your bot server.
3.	Set Up Webhooks:
•	Facebook will send messages that are sent to your page to a webhook of your choice.
•	Set up an endpoint on your server that listens for POST requests.
In the Facebook App dashboard, under “Webhooks”, set up a new webhook with the callback URL pointing to your server endpoint and subscribe to messaging events.
4.	Connect Your Bot:
•	Using the Page Access Token and the Facebook Graph API, set up your server to respond to the messages sent to your Facebook Page.
5.	Review:
•	Before your chatbot goes live, it will have to be reviewed by Facebook. Ensure that it adheres to Facebook’s platform policies.

Design Persona
Name: Eddie (derived from "EventBuddy")
Communication Style:
Casual: Uses a mix of youthful jargon and simple language that resonates with college students..
Informative: While maintaining a casual tone, Eddie ensures that the core information about events is conveyed clearly.
Catchphrases:
"Are you prepared to slay that campus event?"
"I've got the details, so don't miss out!"
"Campus vibes are building up!"
User Scenarios for the EventBuddy Chatbot ("Eddie")
 Freshmen introduction
User: Requests information about important yearly events.
Eddie: Offers a calendar of major college events.
Check the event timing
User: Requests the beginning time of a particular event.
Eddie: Announces when the event will begin.
Location of Event Enquiry
User: Requires instructions or the location of a place for an event.
Eddie: Gives the venue information and provides a map.
Registration for the event
User: Desires to sign up for a certain workshop or event.
Eddie: Provides a link for registration.
Reactions to Events
User: Would like to comment on a recent event and Eddie: Asking the user
User Experience Guidelines for Chatbots
Onboarding: Greet users and introduce the chatbot functions.
Language: Avoid using technical jargon and speak in a nice manner.
Quick responses: Provide a succinct response.
Error Handling: Acknowledge misunderstandings politely and provide solutions.
Offer alternatives or succinct responses to steer talks.
Feedback:  Allow people to comment on the performance of the chatbot.
Human Handoff: When necessary, provide a transition to a human representative.
Context: Remember user preferences or interactions during a session.
Continuous Learning: Keep an eye on interactions and update frequently.
Privacy: Prioritize user data privacy and educate users about data handling.
Control: Make it simple for users to halt or resume talks.
 
Response Configuration For Eventbuddy In Watson Assistant
Intents
•	#ask_event_info
•	#event_registration
•	#ask_event_location
•	#feedback_or_issue
Entities
•	@event_name
•	@event_type
Dialog Nodes
•	Node: Ask Event Info
•	Node: Event Registration
•	Node: Ask Event Location
•	Node: Feedback or Issues
Fallback Node
•	For unrecognized queries or errors:
•	Response: "Sorry, I'm not sure about that. Can you rephrase? Or type 'help' to see what I can assist with."

