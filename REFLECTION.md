************************************************
Check Point Questions:
************************************************

Checkpoint 1: What properties does the planet object have? Write down 3.

Climate: 'arid'
Created: '2014-12-09T13:50:49.641000Z'
Population: '200000'

Checkpoint 2: What status code do you see when the ID doesn't exist?

Request failed: 404

Checkpoint 3: Does the loading message appear before the data loads? It should flash briefly on a fast connection.

the message "loading 'category'...", depending which category you choose it'll say that one is loading.


************************************************
Reflection Questions:
************************************************
1. Compare this async/await version to the .then() chain from the Promises + Fetch lesson. What's actually different under the hood? What's the same?
   When looking at the two they appear to function rather different. However the major differences occur mainly in aappearance. However, within both they fun tion asychronously. Also both async/await still relies heavily on Promise+Fetch in its processing.

2. What would happen if you forgot the if (!resp.ok) return guard and SWAPI returned a 404?
   If the resp.ok is forgotten within the code it continues processing as if the error code wasn't returned. This can lead to further errors within the program.
   
3. Where else in this course have you used a guard clause to exit early? How is this the same pattern?
    Whenever we we're making conditions for our field entries the process was very similar. Within making conditions we'd create the exit early to stop users from being able to enter invalid information. 