---
author: nicklalone
date: 2018-01-14 12:00:00 +0800
title: The Centrality of Objects
categories: [Simulation Observation]
tags: [ANT, Academia, Dissertation, HCI]
---

The Centrality of Objects
=========================

Understanding the measures of Centrality in Association Mapping
---------------------------------------------------------------

In social network analysis, some of the more useful calculations display the centrality of actors and their importance within a network. There are many different measures of centrality and importance. Some centrality measures display how many other nodes a particular node is a part of. Others show how often a particular node is needed when tracing a path from one node to another. Interpreting these measures is contextually based and couched in the way the network itself functions.

At the core of SNA is choice. As such, in some measures the prominance of actors is more important. The prominence of an actor and its centrality may be quite different. For example, in an office environment, there may be a large number of workers who all do the same thing. This entire collection of nodes is central. However, among those, one worker may be more prominent simply because they host far more people choosing to associate with them. In competitive environments like sales, this is an important measure. Additionally, it has other uses for my proposed method of SNA in HCI — association mapping.

Within Association Mapping, these principles are still true — central actors are important. However, where their numeric dependencies are similar, the context and interpretation of these data might be more than a little different. In this section, I outline the four common measures of centrality and their importance to Association Mapping: Degree, Closeness, Betweenness, and Eigenvector Centrality. Each of these types of centrality are directional in nature with directional meaning that one actor is directing a dyadic pairing. In the case of software, users or the software itself may be directing the activity.

Degree Centrality
-----------------

This measure of centrality is perhaps the most simple yet also the most useful within the toolbox of social network analysis. Degree centrality is essentially defined as how many neighbors a particular node has on a network or graph. Another way to talk about this is that degree centrality allows the researcher to learn the most mathematically active actors in a particular network or graph.

Within directional networks like the ones being used for association mapping, the degree centrality is somewhat unique. For example, directional graphs often use the concept of choice to indicate that choice is available and not forced. However, when doing anything social, the nature of choice is something that is not entirely evident. As such, association mapping rests on the idea of making a choice as a base of any actor.

But how is this used within the analysis of data in real time? Well, within directional graphs there are two measures: indegree and outdegree. Or more plainly, how many actors are associating with a particular node and how many actors that node is associating with. Outdegree is the usual measure that most analyses use as it indicates that a choice has been made. For example, consider the nature of bricks in Catan.

With Bricks in _Catan_, the choice is not necessarily made by the brick but instead, is made by the Dice, by the players playing cards, by the terrain that the player’s pieces are sitting upon, and by the numbers sitting on each of those pieces of terrain. Like humans, many of the _choices_ we have are typically little more than reactions toward a particular input. However, as we change modalities — from the tabletop toward that of the iPad — we see the following over the course of a game for the nonhuman objects: Bricks.

![OutDegree Centrality for Brick — Left (Blue) is Tabletop with Right (Orange) as iPad.](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*Hl0xwJ4_GOHyoVLZaIv3Xw.png)

In this chart, we see that bricks are more central to the tabletop game over the iPad game. While we can note mathematically that this is case, we cannot really say anything other than the fact that Longest Road changed hands twice in the tabletop game whereas it was only awarded once in the iPad game. Roads require brick and lumber to build. However, so too do settlements. As such, using centrality is not necessarily the best use of any analysis.

However, what if we were to average the centrality of resources overall between these two modalities? After all, over the course of a game the same number of dice are rolled N times where N is the number of players times the number of rounds in game. With that in mind, the chart for these two games looks like this:

![OutDegree Centrality for Resources— Left (Blue) is Tabletop with Right (Orange) as iPad.](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*TXj30BHYMIxR0xdeZU3pyA.png)

In the above chart, I have plotted the average, normalized centrality for all resources across 16 turns of play. For the tabletop game, the average centrality of all resources was .215829 whereas in the iPad game, the average centrality is .1257. As such, we can say without a doubt that resources did not factor in to, or make as many choices, in the iPad game as they did in the Tabletop game. But why?

Well, this is a relatively simple answer. When players on the tabletop game were in their game, they traded with tangible cards. As such, they would show and hand cards across the table to another player. This meant that Bricks, Ore, Sheep, and all the rest existed physically in the table. For the iPad game, the existence of resources was a numeric quantity that only one player could see at any given time.

Therefore, many of the associations the resources themselves could make decreased. In this case, they decreased by a factor of .092. As these values were calculated with UCInet, we can say that in normalizing these values, UCINet takes the degree of a particular actor and divides it by the maximum possible degree. This results in a percentage which means that there was at least a 9% decrease in average centrality for the resources in a game of _Catan_ when comparing Tabletop vs. iPad.

But this still does not necessarily tell us anything aside from the fact that resources are not as tangible. Where we may find something interesting to discuss via the data is with the humans themselves. Because _Catan_ is a game that requires players to be active, to discuss trades, to relate to all manner of other actor, we can expect a significant amount of human centrality. Through this, we can see the average centrality over 16 turns of _Catan_

![OutDegree Centrality for Humans— Left (Blue) is Tabletop with Right (Orange) as iPad.](https://miro.medium.com/v2/resize:fit:1398/format:webp/1*JMTk9nEFm6N78p-qLZVd_w.png)

In the above, this is the average Outdegree centrality for all human actors between the two modes of play _Catan_ that were recorded. In this particular game of 3 players, the tabletop centrality measure for humans was .556254 or 56% of all activity came from humans. This is compared to .324958 for the iPad game. This means that approximately 32.5% of all activity of the iPad game was performed by humans themselves.

The difference for this type of centrality is approximately 23.1%. Or, on average humans were 23% less central to a game of _Catan_ played via the iPad application. This too, is the result of automation but the implications for this will be described in the analysis section. The next type of centrality for directional graphs is closeness centrality.

Closeness Centrality
--------------------

Closeness centrality of what is essentially the distance between actors is another way to consider a matrix or graph. With closeness centrality, the “closeness” is indicative of speed. For example, what nodes are most central, who will I have to talk to if I want to get to as many different other actors as possible. If an actor is central to a graph, it can reach all other actors with as few jumps through other actors as possible.

With Association Mapping, this is an essential component of the strengths of measuring a design. For example, if in mapping out this tabletop game, I come across the idea that a oarticular aspect of the game is important — like trading in _Catan_ — then my focal point on design will be in lowering the bar for trading in order to have it more accurately reflect that experience that players will bring with them to the app itself.

![Closeness Centrality for Top 10 Non-Human Objects Left (Blue) Tabletop and Right (Orange) iPad.](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*YvJltgyvsFIjE1lbwcAUDw.png)

Between these two games, we see a number of objects that are central to that particular modality. For the tabletop game, the closest non-human objects are the Resources, which humans must distribute to one another. In addition, there is Terrain, which humans must refer to in order to examine the resources. Next are the numbers. Here, humans must examine the numbers attached to the terrain in order to distribute resources. We then see the most common resources of this particular game followed by the winning player’s resources, the dice that determine the numbers and then each other player’s numbers.

The iPad game is a little more complex. The “Check” is the user-interface check mark is present each time a player makes a decision. It is the last item checked before anything occurs. Therefore, it is the most central object and actor. It controls access to computer-mediation. Next, the dice are not the same object as the dice in the tabletop game. Instead, the Dice represent when play is switched to the next player. The “User-Interface” is the terrain and all information related to play. While this screen is important, it is not necessarily central. Resources play another central roll in this game but is primarily disconnected from play.

Interestingly, because the players spoke to each other, their phones, and other disconnected objects during the iPad game, the centrality of the iPad objects are slightly lower than they would normally be for this measure. Additionally, many of the independent objects with the iPad game could be combined for even more robust central objects. The Check mark could also be combined with nearly every other non-human object of the iPad game as it is something that pops up constantly. Overall, the centrality of non-human objects is far less logical than that of the human objects because while computer-mediation is logically based, much of it is invisible. Additional developments with this particular method will incorporate computer logs in order to make these objects more manifest. Next, we will discuss Betweenness Centrality.

Betweeness Centrality
---------------------

Another measure of distance is referred to as “betweeness.” This type of centrality is best explained as the amount of stress a particular actor has to go through to reach some other actor. An example of this can be found in the 1979 article, “The medieval river trade network of Russia revisited.”

> Suppose that in order for _i_ to contact _j, k_ must be used as an intermediate station. _K_ in such a network has a certain ‘responsibility’ to _i_ and _j._ If we count all of the minimum paths which pass through _k,_ then we have a measure of the ‘stress’ which _k_ must undergo during the activity of the network.

Within association mapping, betweeness centrality is partially related to the outdegree centrality but is indicative of the proportion of incoming and outgoing associations. It is here that we might learn of those actors that are the most essential for the task at hand. Take this example from the two games analyzed in the previous section.

![Betweenness Centrality for Humans — Left (Blue) is Tabletop with Right (Orange) as iPad.](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*kTqn9BgoPfTWEtSUjvi2UA.png)

Here, we see that humans are far more central to the action of tabletop gaming. This is not to say that humans are the only movers and shakers of the board but that during play, during an activity, normally humans are central to all activity. When play is mediated by a computer like it is with digital board games, it is often the case by designers that they automate certain aspects of play. In doing so, the centrality of non-human actors increases exponentially in that any measure that seeks to evaluate the impact on the humans will no doubt see a decrease.

To put this as plainly as possible, components of a game do not need to go through human hands in an iPad. They are guided by the iPad itself. For example, the “Check Mark” that is present at each stage of a human’s action has a centrality very similar to that of the humans in the iPad game. Next, we consider page rank or eigenvector centrality.

Eigenvector centrality
----------------------

This form of centrality is essentially one of influence. When an eigenvector analysis is performed, whatever program being used to perform the analysis assigns scores to each actor within a network. These values are as such that those with high values are essentially contribute more than those nodes around them. Another way to think of eigenvector centrality is page rank. With page rank algorithms like those by Google or other search engines, page rank accounts for how many links go to certain pages. Those with high numbers of links going to a page are essentially providing a sense of how “important” that page is.

UCInet calculates eigenvector centrality. These again are normalized as a percentage. In continuing with the examples above, here is a plot with the eigenvector centrality of the humans in each game type.

![Eigenvector Centrality for Humans — Left (Blue) is Tabletop with Right (Orange) as iPad.](https://miro.medium.com/v2/resize:fit:1338/format:webp/1*bLOCaAhozRovzx12AZ9pEA.png)

Here, we see that humans remain immensely important within the activity itself. Of all nodes in these networks, they are the more important or essential aspects of a network. Again though, the importance leans toward the tabletop game in that there is an average, overall eigenvector centrality of around 87% for the humans. For the iPad game, that eigenvector centrality lowers to 82%. This again, is accounted for by the automated aspects of the game that humans no longer have to manually do.

All of this is evident by examining the network structure visually as well. Take these two plots.

![captionless image](https://miro.medium.com/v2/resize:fit:1000/format:webp/1*n3qBIPADURIoMZZY-Pn7yQ.png)![The network of play via tabletop of the left as opposed to the network of play of the iPad on the right.](https://miro.medium.com/v2/resize:fit:1000/format:webp/1*IzrePIDrSxkgo49aOseuow.png)

Note that within the tabletop game (left) that the network itself is highly centralized. The human players are maintaining the system by using the tools of the activity to do so. On the right, on the other hand, there is a secondary network of actors that are loosely connected to the central space. This is the computer-mediated aspect of the network visualized for the entirety of either game. Taken per turn, this visualization is still noticeable, just not as starkly.

In the next section, data analysis begins. I will start by summarizing the larger trends that can be seen among all the games analyzed. Once summarized, each trend will be broken down in to how it manifested across each game and how each game, with their own unique contexts, displayed similarities. After breaking down each trend, I will offer a concluding section on what each of these concepts means for design. After discussing the implications for design, I will finish by offering a design fiction that describes a world of design and use that highlights the benefits of association mapping.
