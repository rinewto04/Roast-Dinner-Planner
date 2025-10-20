# Roast Dinner Planner
Building AI course project
Idea for a software that uses AI methods to optimize and inform you of the cooking timings for the various components of a roast dinner and comes up with a timing plan so it's all ready at the correct time.

##Summary
This software will optimize the cooking timings for the various components of a roast dinner and come up with a timing plan so it's already at the correct time.

##Background
General Description
Roast dinners typically require a fairly standard set of components with some variations. However, depenedent on the number of people you are cooking for, the size and type of meat joint, and the various sides you choose to serve it can be chgallenging to ensure all the food is ready at the correct time so it is all warm and ready to eat at the same time.

An ideal roast dinner is all ready simultaneously and cooked perfectly

##Possible Deviations
The algorithm may choose to deviate from the ideal order in the following ways:

Keeping some sides out of the oven where their eating temperature is more variable than say the meat
Precooking some components and then rewarming them.
Over or undercooking parts of the roast
Penalties will apply for plans that involve repeated cooking and rewarming or parts of the meal that are cold on serving

This list might be extended in further development.

##Possible Inputs
The algorithm will need an input for the size and number of shelves in each persons oven as well as which elements of the roast they want to cook and for how many people. 

This list might also be extended in further development.

##The Valuation Problem
It is unclear how the penalties should be balanced but rewarming food seems less of an issue than food being cold. Therefore, foods with less issues with being rewarmed would be prioritised in the cooking schedule. 

The AI could work by utilising two different layers:

The Ideal Layer expects as input all the roast data described above and outputs an ideal ordering of the time each component should be put in the oven for optimal serving time.
The Valuation Layer will use the input data on oven size and configuration described above and penalty valuations, and will try to reduce the penalties by choosing them according to an algorithm and presenting the corresponding optimal cooking order and time to the user, who can give their feedback. The user can thus train the algorithm to guess penalties that match the user's preferences.

##How is it used?
First, the user has to input all the data about the oven and roast they are cooking. Then they will have to rate different cooking orders and timings.

The penalties should be stored and used as a starting point for later arrangements.

##Data sources and AI methods
This algorithm would need data specific to cooking roasts, such as:

Recipes and timings for the various possible components of a roast dinner
the dimensions of the oven, number of shelves, and possible distances between them 
The AI methods used for this project are probably genetic algorithm, simulated annealing, and reinforcement learning

##Challenges
Challenges in Implementation
The data model for the shelf might be challenging to implement in a way that allows for efficient optimization and not continuous changing of the shelf set up during cooking

Challenges in Using oven and shelf data
The biggest challenge is balancing the amount of data entered with the time to input it. If too onerous people might rather choose to just give it a try on their own. A slightly simpler but less ideal situation with more limited informatuion may be more useful for people.

##What next?
These are the next steps:

Gather data for testing.
Develop a prototype.

Acknowledgments
Thanks to the “Building AI” course which forced me to come up with this idea.
