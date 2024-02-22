# Post-Office-Delivery
This was a school project written in Python, where we coded a delivery truck simulation. This project was split into two parts: setting up the basic data structures, and delivering the packages as fast as possible given a map.

# Note: I am not providing the code due to University restrictuions. 

# Part 1
Part 1 involved completing an unfinished program which would initialize our simulated truck. In this program, we needed to set up methods that enabled our truck to collect and deliver packages at a given location, as well as return a package to a post office without delivering it. The truck also needed to be able to drive from one location to another, and return a list of all of the ids of the packages on the truck at any given time. 

Packages could be initialized and given an id, delivery address, and a post office from which it belonged. They also had classifiers to record whether or not they had been collected and delivered. 

The truck could be given an id, a size (of how many packages it could hold), a starting location, an empty list to record which packages it had, and a counter for mileage. The truck was able to "collect" a package from a post office, so long as it was at the correct post office and had enough room on the truck. It could then deliver the package if the truck was at the delivery address of the package. The truck could also remove packages from its storage when at a post office. Finally, the truck had a function to drive to a new location, which would add the mileage to the truck, and set the new location.

# Part 2
Part 2 was the real meat and potatoes of this exercise. This simulated the actual delivery service of the truck, and necessitated the truck to follow a map of nodes, of which every single one was not connected to another. This utilized a Breadth First Search to determine a driving route from point A to point B, picking up and delivering packages along the way. It utilized all of the methods that we established in Part 1 of the project, and returned a pair of where all of the packages were delivered to, and the stops the truck made along the way. The inputs for this function were the given map, our truck, and the list of packages and the post offices that they were located at. 

Our truck was able to read the map, pick up the packages it needed to, and drive to and from the required locations in order to complete its delivery route. 
