# Jeyaditya_Y1_U1_SA
A campus bot that gives you directions from the gate, what the canteen can offer, the offices location and the seminars that happen.

•	Student name: Jeyaditya . A 

•	Registration number:100406 

•	Course name: Artificial intelligence real world application and implication. 

•	Link for Chatbot: https://jeyaditya.github.io/IDAI101_100406_Jeyaditya_Y1_U1_SA/


IB Campus Bot – Project Documentation
1. Introduction
The IB Campus Bot is a virtual assistant created using Dialogflow ES. It is designed to help students, teachers, and visitors navigate an International Baccalaureate (IB) school campus. Instead of asking people for directions or office timings, users can simply chat with the bot to quickly get the information they need.

The bot can answer questions such as:
- Where is the IB Office?
- What are the library timings?
- When is the next CAS Fair?
- How do I get from the East Gate to the Cafeteria?
- Who can I call in case of an emergency?

By automating these everyday queries, the bot saves time and makes the campus experience smoother for everyone.
2. Why I Built It
My goal was to design a chatbot that feels helpful, reliable, and easy to use. I wanted it to reflect a typical IB school environment, so it includes the CAS Office, TOK Room, library, auditorium, hostels, and sports facilities.


3. Entities (The Bot’s Knowledge Base)
Entities are the building blocks that tell the bot what words to recognize. For example, if a student asks about 'Library' or 'Science Block', the bot knows these are campus buildings.
I created entities for:
- Buildings: Admin Block, IB Office, Library, Science Block, Arts Block, Sports Complex, Cafeteria, Auditorium, CAS Office, TOK Room.
- Departments: DP Office, MYP Office, PYP Office, Computer Science, Mathematics, Sciences,     Humanities, Languages and Business.
- Events: Orientation, Seminar, Workshop, Examinations, CAS Fair, TOK Exhibition.
- Days of the week: Monday to Sunday.
- Transport: Bus, Metro, Auto, Cab.
- Campus zones: North Gate, South Gate, East Gate, West Gate.
- Offices: Admissions, Examination Cell, Accounts, Counselling, CAS Office, TOK Room.
- Roles: IB Coordinator, HOD, Counsellor, Librarian.
- Hostels: Boys Hostel, Girls Hostel .
- Sports: Cricket, Football, Basketball, Badminton, Swimming.
4. Intents (What the Bot Can Do)
Intents are the actions the bot takes when it recognizes what the user wants. For example, if a student types 'Where is the library?', the bot matches this to the 'CampusLocation' intent and responds with directions.

Here are the main intents:
- Welcome: Greets users and explains how the bot can help.
- Fallback: Responds when the bot doesn’t understand.
- CampusLocation: Shares building locations.
- DepartmentInfo: Gives details about departments and offices.
- OfficeHours: Tells when offices are open.
- LibraryHours: Library timings.
- CafeteriaMenu: Example daily menus.
- EventsToday: Lists events happening today.
- EventLocation: Shares where events are held.
- TransportOptions: Provides details about buses, autos, cabs, and metro.
- HostelInfo: Information on hostels.
- SportsFacilities: Details of sports facilities.
- DirectionsFromGate: Step-by-step guidance from a gate to a building.
- TimetableQuery: Class times for different departments.
- EmergencyContacts: Important numbers and medical room info.
- ContactHuman: Phone/email details for reaching a person directly.
5. The Webhook (Brain of the Bot)
While most answers are pre-written, some responses are generated dynamically using a webhook. The webhook is a small Node.js server that can give customized answers, like combining the gate and building names into clear directions.

For example:
User: How do I go from West Gate to the Library?
Bot (via webhook): From West Gate, follow the main avenue for 200m, then turn right to reach the Library.

These webhooks require payments to be active all the time so they are being disconnected for now, the webhook was created through Replit, and Github using Python 3.13 .


6. Future Improvements
Some features we plan to add include:
- Supporting multiple languages, since IB schools are multilingual.
- Linking with live school systems for real-time timetables and event updates.
- Adding voice integration for Google Assistant and other platforms.

7. Integration details:
  I have integrated my chatbot through the dialogflow messenger and added it into an empty website for usage.

8. Final Thoughts
The IB Campus Bot is now ready for use. It covers the most common questions asked around an IB campus, while the directions part is a bit too vague. This project shows how AI can make daily school life more convenient and connected.

