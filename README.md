# usfx.hashtable

### Implementation of the hashtable in the class ci583.ass1.htable.Hashtable.java. 

1. When a new Hashtable is created, the array should be initialised with a size which is the smallest prime number larger than or equal to the requested initial capacity. 

2. The default probe type should be LINEAR_PROBE. 

3. Store objects in the array using the Pair class to store both key and value. 

4. When storing a new key/value pair, use the findEmpty method to find an unoccupied location starting the search at the value found by hashing the key and with a stepNum of zero. If this position is occupied, use the getNextLocation method (which is implemented for you) to find the next location to search based on the probe type being used, and call findEmpty again with the new location. 

5. You will also need to use the getNextLocation method when implementing find, which searches for an existing value – again, start the search at the value calculated by hashing the key. If there is no Pair object at that location, the key was not found. 

6. If there is a Pair object at that location then either its key matches the one we're looking for, in which case return the value associated with the Pair, or it doesn't match. If it doesn't match, we need to find the next location to search using getNextLocation, and call find again with this new value
'''
