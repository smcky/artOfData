---
layout: post
title: Digimon Lab Results!
subtitle: A lab by Sarah Cohen
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [test]
author: Sarah Cohen
---

**Lab Results**

| Avg Speed of all Digimon | Total Number of Digimon of Type | Example Team of Three Digimon with Atk ≥ 300 & Memory ≤ 15 |
| :------ |:--- | :--- |
| 120.40160642570281 | 82 | team: ['Lopmon', 'Wormmon', 'Vegiemon'], 'total_memory': 14, 'total_attack': 308 |

I wrote three functions: one to take the average value of a specified property, one to count the total number of Digimon with a specific property value (like Type = Vaccine), and one to create teams based on Memory allotments.

All of these needed slightly different data structures to effectively handle the data in order to produce the desired output; for example, to take the average speed of all Digimon, I added each speed value to a list, then used statistics.mean() to take the average of every entry in the list, whereas I stored each team of Digimon as a dictionary. 

At first it was sort of difficult to figure out how I was going to need to change the basic setup of my code from the handing the favorite_colors and penguins data to this, but I realized it was just easier to make individual functions with different data structures for each task since the tasks had gone up in complexity. I also needed to figure out how to find all possible teams given specific requirements, for which I had to use the itertools.combinations() function.
