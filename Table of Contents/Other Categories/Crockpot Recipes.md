---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[crockpotbanner.jpg]]"
banner_y: 0.912
---
# Crockpot Recipes

Featuring a collection of easy, hands-off meals that are perfect for busy days. With minimal prep, you can set it and forget it, allowing the slow cooker to work its magic while you go about your day. From comforting stews and soups to tender meats and flavorful vegetable dishes, these recipes are designed to deliver delicious, hearty meals with little effort. Ideal for lunch or dinner, crockpot meals offer the convenience of having a warm, satisfying dish ready when you need it, making it easier than ever to enjoy homemade comfort food on even the busiest of days.

There are `$= dv.pages("#crockpot").length` crockpot recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #lunchdinner_recipe and #crockpot and -"Templates"
SORT file.name ASC
```



```meta-bind-button
label: Back to Main Menu
icon: "book-open-check"
hidden: false
class: navigation-buttons-center
tooltip: ""
id: menu-button
style: primary
actions:
  - type: open
    link: "[[Menu]]"

```
 
