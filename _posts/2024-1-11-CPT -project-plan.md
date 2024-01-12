---
toc: False
comments: True
layout: notebook
title: CPT Plan
description: Binary CPT Project Review Ticket
type: tangibles
courses: {'compsci': {'week': 4}}
---

# Frontend (Vance, Ashwin, and Dante)

## Ashwin
I will be in charge of creating the SASS and style formating with vance. I will also help with the API integration for my deck builder. I want it to be able to anyilize the stats of all of the card from our backend api, along with online apis, such as Royal Api, to acsess popular decks. My feature will also give winrates or other statistics based on the deck.

## Vance
I will be in charge of most of the frontend visual style and color scheme with constructing the interative elements such as tables and dragable objects with their correct styling. This will utilize my knowledge of html for the visual elements and mixed my java knowledge to create moveable tiles and interactive elements to engage the viewer. This will tie in with Ashwin and Dante's features impriving the user interface and making them function. I will also help the backend developers when neccesary as we are a 5 person team, and I have experience from my last team on backend. 

## Dante
My feature will be a card collection and potentially like and dislike certain cards and decks submitted by users. The likes and dislikes could be stored in the back end where the users specific likes and dislikes are stored. Also, the card collection I beleive this could be stored in a sq lite database connected with lincoln database. I woud have to work on integrating the backend to the front end so the users frontend information gets stored with lincolns.

# Backend (Lincoln and Gurshawn)

This website is designed for Clash Royale enthusiasts, providing a platform to select cards from the game, create personalized decks, and share them with the community. Users can publish their decks, allowing others to view, rate, and add public comments. The interactive aspect encourages strategic discussions and the exchange of ideas among players. The platform offers both light and dark modes to accommodate user preferences. Users also have the option to store their decks privately for personal use or share them publicly, contributing to the collective knowledge of Clash Royale strategies. Overall, the website serves as a hub for users to explore, rate, and discuss various Clash Royale decks, enhancing the gaming experience for the community. To enhance functionality and user interactivity, APIs are employed to fetch and display Clash Royale card data in real-time. This ensures that users can seamlessly select and integrate the latest cards into their decks. The integration of APIs also enables dynamic updates, ensuring that the platform remains current with the ever-evolving Clash Royale card pool.

User Authentication:

Implement a system for users to securely create accounts.
Develop a login mechanism for user authentication.
Database:

Choose and set up a suitable database system (e.g., MySQL, PostgreSQL, MongoDB).
Design the database schema to store card data, user ratings, and deck information.
Card Data Structure:

Define attributes for card data, including name, type, description, image, etc.
Establish relationships between different components of card data.
Rating System:

Develop a user-friendly rating system.
Associate user ratings with their respective accounts.
Deck Management System:

Enable users to create and store decks.
Define deck attributes, including name, description, and associated cards.
User Interface (UI):

Create an intuitive and responsive UI for card and deck management.
Ensure compatibility across various devices.
Search and Filter Functionality:

Implement search and filter options based on card and deck attributes.
Allow users to refine card and deck selection based on criteria like type, rating, and name.
User Profiles:

Allow users to manage both rated cards and created decks within their profiles.
Provide features for viewing activity history and customization.
Security:

Implement security measures, such as encryption, to protect user data.
Use secure connections (HTTPS) to prevent unauthorized access.
Notifications:

Incorporate notification features to update users on new cards, changes in the system, or deck-related activities.
Allow users to customize notification preferences.
Moderation:

Implement a moderation system to handle inappropriate content.
Verify user ratings and deck content to maintain system integrity.
Feedback Mechanism:

Provide a user-friendly way for users to provide feedback.
Establish a reporting system for users to flag issues related to cards or decks.
Performance Optimization:

Optimize site performance for quick loading times.
Address scalability concerns, especially with a growing number of cards, decks, and users.
Testing:

Conduct comprehensive testing to identify and rectify bugs.
Test usability from different user perspectives to enhance the overall user experience.
Documentation:

Create clear and concise documentation for users.
Include developer documentation for understanding site usage, APIs, and deck creation.

