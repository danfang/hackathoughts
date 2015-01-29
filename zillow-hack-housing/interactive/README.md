# Interactive Housing Search

## Design/Flow

### Summary
Extremely simple fade-in, fade-out scrolling dialogue to query for the right real estate.
High emphasis on design, simplicity and conversational nature. Gives the option to skip any
question (except location) for a broader breadth search.

### Dialogue
Question 1: I want to live near...

Rep: Google Maps API to drag or draw an area on the map (replacing the "near" or "radius" search options)

Question 2: Do I want a new property? 

Rep: Yes/no/idc buttons.

Question 3: How much am I willing to pay?

Rep: Slider with a min and max

Question 4: What type of house am I looking for?

Rep: Show icons of house, apt, duplex, condo, etc, check boxes

Question 5: What amenities are important to me?

Rep: A dynamic list (can add items) of local attractions, e.x. Gym, UW, Trader Joes, etc.

Implementation: For each item in the list, query and map the items found for that list. Find the shortest weighted avg of distances from these nodes.

### Results

Display the list of query parameters, with the ability to delete or alter them to perform a new query.

Rate each "acceptable" house based on qualities of the user's query, ex:

- OVERALL: 4.3/5
- 3/5 price (far away from mean)
- 5/5 location
  - (star) close to UW
  - (star) close to Gold's gym
- 5/5 type (is a new house or condo or apt)
