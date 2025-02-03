I tried to add the ability to switch between milliliters and grams throughout the entire website, so it would display one or the other on each ingredient. I was surprised that this didn't work, given the complexities of the previous features it added. 

It is reasonable because, to my limited cooking knowledge, mls and grams are interchangeable, and having the user be able to choose their preference would've been nice.

When a menu on the top right was flipped from grams to milliliters or vice versa, everything on the screen would change accordingly. So if it said "30 g Cream" and the menu was switched to milliliters, then it would say "30 ml Cream."

The reason why it was implemented wrong, as per chatGPT, is:

The problem is that while the calculations are correct, your implementation does not handle the text changes properly for the units, specifically for ingredient labels and the displayed unit next to the total drink size. The reason your current code isn't working as expected is that the unit change is not propagated throughout all the relevant labels on the page.

To fix this, you need to ensure the text content for each unit (grams or milliliters) is updated in the following areas:

Total Drink Size Display: The total drink size should update with the correct unit (ml or g), but it's currently only updating the value without changing the unit label.

Ingredient Labels: When the unit is switched between grams and milliliters, the displayed text for each ingredient (e.g., matcha, water, ice) needs to update as well.