We would like to design an advanced Gen-AI chatbot. This chatbot will be the primary interface for interaction, facilitating tasks like customer support, handling sales inquiries and tracking orders.

* **Chatbot Features**
- The chatbot should be capable of handling customer support tasks, answering sales inquiries and tracking orders seamlessly.

* **User Interaction**
- The chatbot needs to be user-friendly.

* **Database Interaction**
- The bot should interact with  MySQL database to extract data when needed. 


* **Sample QA**
User: What is Address of my customer whose name is TechnoSystem.
ChatBot: You have a customer whose name is “Techno Systems PvtLtd”. Its address is: Rodas Enclave, Park Ln, Hiranandani Estate, Thane West, Thane, Maharashtra 400607.

User: How many customers are inactive since last 2 months
ChatBot: There are 4 customers who have not purchased any material from our crusher

User: Give me their names
ChatBot: 1. ABC, 2. PQR, 3. RST, [login to view URL]

User: do we have any outstanding from them?
Chatbot: Yes. ABC has an outstanding of 2,25,000Rs, while PQR, RST and XYZ don't have outstanding

User: Give me the names of our top 2 clients.
Chatbot: AMR pvt Ltd is our top client with a business of 1,23,45,122 Rs. While second top client is RamBhav with a business of 56,45,000Rs

Ultimately, the goal is to create a chatbot that is a valuable asset to our software, streamlining operations and enhancing the user experience for both customers and Stone Crusher owners.



Admittedly, with the simple instructions, I think we can focus on creating a chatbot that is not terribly sophisticated but is capable of tapping into a DBMS. The latter may be achieved with sqlite3, connecting to the database and then fetching relevant data.

Since we need very simple replies that only vary in the specific details retrievable from the databse, we can simply program the bot to respond with a set combination of phrases to specific operator questions, rather than
expend resources on NLP which may not even deliver the desired reply. 
