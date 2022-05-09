# Rimworld sell or smelt calculator
 
This calculator is made to help Rimworld players determine whether it is more valuable to smelt an item to gain some resources from it, or wait to sell it.
It complements https://rimworldwiki.com/wiki/Electric_smelter#Sell_or_Smelt section of official Rimworld wiki.

Can be used online on Github Pages https://demak.github.io/Rimworld-sell-or-smelt/.
 
## Usage instructions
 
Page is divided in two sections - a smaller settings section on the right and a bigger section with a list of items on the left.
Settings section allows you to set every modifier which affects trade prices according to your current in-game situation. This will affect how profitable it is to sell items and buy resources and thus whether it is more profitable to sell or smelt items.
 
List of items will show items selected in the settings section with price and hit points percentage at which it is profitable to sell items displayed for each quality level. It is assumed that it is more profitable to sell an item if it can be sold for more silver than will be spent to buy resources received from smelting an item. Each quality level will display hit points percentage at which item's sell price is equal to buying price of smelt materials. Thus at higher hitpoints selling price will be higher, while at lower hit points selling price is lower than buying materials.
 
### Detailed settings description:
 
All settings are related to modifiers which affect trade prices, all of them are described at https://rimworldwiki.com/wiki/Trade_Price_Improvement
 
1. Difficulty level price disadvantage: Higher difficulty levels impose disadvantage to buying and selling prices. Higher price disadvantage will substantially decrease prices for selling items and increase resources buying cost, making smelting more important than selling.
 
https://rimworldwiki.com/wiki/AI_Storytellers#Difficulty
 
There are four options available:
- Strive to survive or lower difficulties have no price disadvantage
- Blood and dust has 10 percents price disadvantage
- Losing is fun has 20 percents price disadvantage
- Custom percentage input - this will display current percentage if any of the above options are selected and you can also enter custom value if your game is set to custom price disadvantage.
 
Settings below allow to set information about the pawn you want to make a trade with. Those should be set according to that specific pawn's state.
 
2. Your trader's social skill: skill of the pawn who will make a trade. Higher skill will make selling items and buying materials more profitable. Usually you should trade with the pawn who has the highest social skill. https://rimworldwiki.com/wiki/Skills#Social

3. Trader has health problems: this should be used only if your pawn has injuries affecting their talking and hearing. Lower talking and hearing will apply a small disadvantage to prices. Checking this checkbox will display two additional inputs:
- Your trader's talking ability percentage: this should be set to current percentage of pawn's talking ability https://rimworldwiki.com/wiki/Talking
- Your trader's hearing ability percentage: this should be set to current percentage of pawn's hearing ability https://rimworldwiki.com/wiki/Hearing

4. Trader is inspired with Inspired trade: check this checkbox if your pawn has an "inspired trade" inspiration. This provides a very significant increase in item price, but is rarely available https://rimworldwiki.com/wiki/Mental_inspiration#Inspired_trade

5. Trader is selling to a foreign settlement: check this checkbox if you are going to send a caravan to sell items to another faction's settlement, instead of selling them to the caravan on your own map tile. This provides slight price improvement.

6. Trader has a Psychic reader (Royalty DLC): check this checkbox if you have a Psychic reader https://rimworldwiki.com/wiki/Psychic_reader installed on your pawn. If the checkbox is checked, psychic sensitivity input will be displayed below, enter psychic sensitivity of your pawns in the input. Psychic reader provides trade price improvement based on your pawn's psychic sensitivity.

7. Trader has a leader role (Ideology DLC): check this checkbox if your pawn has a leader role provided by your ideology https://rimworldwiki.com/wiki/Ideoligion#Leaders.
 
## Using offline
 
Whole page is organized into a single .html file, making it easy to use it offline. The only dependency is a Vue.js library, which is used to provide dynamic updates, also included into the .html file and thus calculator can be used without internet connection. Download or save raw copy of index.html file from Github to use it offline.
 
Unfortunately saving a page through Ctrl+S, when viewing a page on Github pages, is not saving all attributes properly and breaks dynamic updates, you have to download it from github.