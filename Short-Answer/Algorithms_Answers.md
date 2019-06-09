Add your answers to the Algorithms exercises here.

Exercise I

a) O(n) - I think this is linear since it starts at n^2 to get to n^3. The running time will increase with the size of the input.

b) O(n^4) - because there are 4 nested loops, each with O(n).

c) O(n) - because it is being called recursively n times before reaching the base case.


Exercise II

1. A naive approach would be to begin dropping eggs starting at the bottom floor and working our way up to floor f where the egg finally breaks. This would have a runtime complexity of O(n). The number of eggs dropped would grow with the number of floors in the building.

2. Maybe a better approach would be to use binary search and find the middle floor in the building and drop an egg from there. 

    If the egg breaks then we an determine that the bottom half contains floor f and we could go ahead and find the middle floor of the bottom half of the building. We continue in the same manner until we find the floor that is one floor lower than floor f at which point the egg doesn't break. 

    If the egg doesn't break at the first half of the building, the we do the same with the floors on the higher half until we find floor f. 

    Since binary search has a runtime complexity of O(log n), I think this will have a runtime complexity of O(n log n).