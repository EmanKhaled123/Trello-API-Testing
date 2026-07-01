# Trello API Testing

I built this project while learning API testing to practice 
working with a real REST API from scratch.

The idea was simple — use Postman to automate the full 
lifecycle of a Trello board: create it, set it up with 
custom lists and cards, then clean everything up through 
the API without touching the UI at all.

## What I tested

- Creating a board and saving its ID automatically for later requests
- Fetching the default Trello lists (To Do, Doing, Done) and archiving them
- Creating two custom lists: Backlog and Completed
- Adding cards to each list
- Deleting all cards, archiving the lists, then deleting the board entirely

## What I learned

The biggest thing was request chaining — saving IDs from 
one response and automatically injecting them into the next 
request using environment variables. Once that clicked, 
everything started to flow.

## Tools
- Postman
- Trello REST API
- JavaScript for test assertions

## How to run it
1. Import the JSON file into Postman
2. Create an environment with your own `API_KEY` and `Token` from Trello
3. Run the collection using Collection Runner with a 2000ms delay between requests

## Results
18 requests — 0 failures
