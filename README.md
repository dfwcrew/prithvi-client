## Inspiration
The biggest challenge that humans are facing today is towards sustaining our planet Earth as we know. Human activities are ignorant of the fact that it is causing an adverse impact on Earth. This has a lot to do with our habits and how small things can cause irreversible changes in this complex ecosystem. Our app is focused on spreading awareness among people by letting them make decisions and see the consequences those lead to in earth's future. For example, increased carbon footprint leads to global warming, which leads to melting of ice and rising sea levels which have the potential to drown several coastal cities around the world. These changes from one part of the world affect the other parts leading to a phenomenon known as "butterfly effect". We try to present this as a game to spread awareness about effects of climate change.

## What it does
Prithvi simulates earth's climate and disasters in the form of a game where users decide on various policies which in the long run can lead to or alleviate a natural disaster. The occurrence of the catastrophe is then plotted on a timeline. Based on the decisions made either the event can happen faster or could also be limited.

## How we built it
We collected climate data (temperature, precipitation), sea level trends, elevation, CO2 and greenhouse gases emission and applied several machine learning techniques (linear regression, decision tree) to come up with a model to forecast drowning of coastal cities across the world. The data is then stored in a database in AWS RDS. A python based REST API connects to this database and plots it in world map and timeline. Each of this event occurs as the time progresses. The backend is deployed on Heroku and frontend is deployed on Azure.

## Challenges we ran into
- Finding the right data set to satisfy the requirements
- Disparate data with a different level of granularity in terms of time and scope- 
- Data cleaning, extraction, transformation, and loading into database
- Feature selection for machine learning models to be effective and it required a well-thought process to predict the outcome correctly
- CORS - Enabling CORS turned out to be a challenge which was convoluted to fix
- Building the timeline with animation turned out to be more complex
- What we learned
- Building timeline was not easy we ran into many bugs and had to figure out a way to make an event occur on map and timeline synchronously.

## Tech Stack
- Front End: HTML5, CSS3, JS, Bootstrap.
- Back-end: Python-flask

## What's next for Prithvi
-Feature addition and fixing minor bugs.
