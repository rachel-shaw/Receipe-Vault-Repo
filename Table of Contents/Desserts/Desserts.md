---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[dessert2.jpg]]"
banner_y: 0.368
---

# Dessert Menu

The dessert section of this cookbook is filled with tempting treats that offer the perfect ending to any meal. From rich, decadent cakes and pies to light, refreshing options, these recipes cater to every sweet tooth. Whether you're looking to impress guests at a special event or simply treat yourself to something delicious, you'll find a variety of desserts that are as fun to make as they are to eat. Each recipe is designed to bring joy to your kitchen, offering a balance of flavors and textures that are sure to satisfy your cravings.

There are `$= dv.pages("#dessert").length` dessert recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #dessert and -"Templates"
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
 
