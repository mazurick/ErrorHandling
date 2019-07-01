# ErrorHandling
Here I'm exploring modelling and throwing errors.

I have a struct named Parser whose job is to deconstruct information from the web. The incoming data can be nil, keys may not exist, and values might be nil as well.

In the body of the parse function, if the data is nil, I throw the EmptyDictionary error. If the key “User Record“ doesn't exist I throw the InvalidKey error.

I obtain a list of keys in the dictionary using the keys property which returns an array. I then use the contains method on it to check if the value exists in the array.

I use a basic implementation of a do/catch statement. 
