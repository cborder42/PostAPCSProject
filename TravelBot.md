# Trip Planner Proposal
We will be creating a travel bot who will help plan a trip based on user preferences. The user will input several aspects of their trip they would like, and the bot will generate a destination. There will be a pool of destinations, each with a set of attributes that the user can choose from, based on user input, the bot will output a destination matching the attributes specified. Additional destination information will show up as well to aid the trip planning. The bot will perform several tasks that will be approved by the user through confirmation messages. 

1. destination
    - pool of destinations with attributes (array?)
        - warm/cold
            - temperature of destination (packing list)
        - country/city
        - near/far
            - calculate distance
            - transportation (plane ticket, train ticket, car rental) 

2. length of stay
    - offer itinerary events
        - add time based on that
        - return total recommended time
