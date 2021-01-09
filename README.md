# Degrees-of-Separation

BACKGROUND

According to the Six Degrees of Kevin Bacon game, anyone in the Hollywood film industry can be connected to Kevin Bacon within six steps, where each 
step consists of finding a film that two actors both starred in.
In this project, I try to find the shortest path between any two actors by choosing a sequence of movies that connects them. For example, 
the shortest path between Jennifer Lawrence and Tom Hanks is 2: Jennifer Lawrence is connected to Kevin Bacon by both starring in “X-Men: First Class,” 
and Kevin Bacon is connected to Tom Hanks by both starring in “Apollo 13.”
We can frame this as a search problem: our states are people. Our actions are movies, which take us from one actor to another (it’s true that a movie 
could take us to multiple different actors, but that’s okay for this problem). The initial state and goal state are defined by the two people 
I am trying to connect. By using breadth-first search, the shortest path from one actor to another can be found.

UNDERSTANDING

The distribution code contains two sets of CSV data files: one set in the large directory and one set in the small directory. Each contains files 
with the same names, and the same structure, but small is a much smaller dataset for ease of testing and experimentation.

Each dataset consists of three CSV files. A CSV file, if unfamiliar, is just a way of organizing data in a text-based format: each row corresponds 
to one data entry, with commas in the row separating the values for that entry.
