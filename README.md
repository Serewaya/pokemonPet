# About
PokePet is a virtual pet simulation with a pokemon theme. In this simulation you will be able to take care of one of three starter pokemon, Charmander, Bulbasaur and Squirtle. Instead of going out to fight different pokemon you will learn how to be a good pokemon trainer and properly take care of your pokemon! So play PokePet and learn about a different aspect of the pokemon universe.

# How to Play
The simulation starts with two buttons on the screen used to switch between different choices of a background and to select a background. Click the next button on the lower right of the screen to switch between different choices or click the select button in the middle to select a background.

After you have selected a background a Charmander will pop up. Just like in the last selection event there will be two buttons, one to select a pokemon and another to switch between pokemon. Like before click the next button in order to switch between pokemon and the select button to select one. 

Once you have selected a pokemon a bunch of objects will be added to the bottom of the screen, a bowl of food, glass of water, box of toys, and toilet. In order to do the corresponding action for your pet simply click any of the objects and the stats of the pokemon will change. If you want to see the stats of a pokemon click the stats button that would be to the left of them.

You will be notified when the pokemon is either hungry, thirsty or needs to dispose of waste by notices coming to the screen, these notices disappear after 10 seconds so pay attention to make sure you don’t miss them!

## How Stats are Measured
Each pokemon has 5 main stats:
- Hunger
- Thirst
- Waste
- Energy
- Health

Hunger is essentially how hungry the pokemon is, it starts at 0 and doesn’t have an upper bound. The hunger of a pokemon is reset whenever you feed them by clicking on the food object.

Thirst is how thirsty a pokemon is, it starts at 0 and doesn’t have an upper bound. The thirst of a pokemon is reset whenever you give them water by clicking on the water object.

Waste accumulates based on how many times a pokemon is fed or given water, it starts at zero and doesn’t have an upper bound. The waste is reset whenever you allow them to go to the washroom by clicking the toilet object.

The energy of a pokemon is essentially how much fun they are having, this stat starts at 100 and doesn’t have a lower bound. To bring up the energy of a pokemon click the box of toys object.

The health of the pokemon is how healthy they are, once a pokemon has a hunger or thirst over 50 health starts going down from the default of 100. If a pokemon’s health gets to 0 they will die. However health can be brought back up since once a pokemon begins to have low energy or health a stethoscope will be added to the world which you can click to bring both stats back to 100.

## Tick Method
The tick method is method that all objects within the world have access to, it measures the passing of time in seconds. First a time function saves a time in milliseconds, subtracts that from the current time in milliseconds and divides the result by 1000 in order to get the seconds that passed. The tick method then adds one to a variable of time every one second that has passed. 

# Pokemon (Inheritance)
All three pokemon inherit from the Pet class which inherits from the Time class. They are all given access to a tick method and functions to know whether the pokemon is hungry, thirsty, bored or needs to dispose of waste.  The Pet class aso has a feed, drink, play and bathroom functions which allow for them to bring up their stats!

## Personalization
All three pokemon have something that they put the most importance on which causes them to become angry when you are negligent of them:
- Bulbasaur is a pokemon that really doesn’t like when he is hungry, so he prioritizes hunger over all the other stats.
- Charmander is a pokemon that can’t stand boredom so he prioritizes energy over all the other stats.
- Squirtle is a pokemon that can’t stand thirst so he prioritizes the thirst stat over all others.
