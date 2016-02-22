---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?
A hash is a collection of Key-Value pairs, similar to an array.


# What are some examples of information that would be Hashes as opposed to some other data type?
Hashes are similary to dictionaries in that they store associated data. For instance a hash might describe a person, who has a name, weight, and height. Each of these traits would be stored as a key, and paired with their associated value, the person's actual name, weight, and height. 


# How are Hashes and Arrays similar? How are they different?
Similarities
   1. Both are used to store a collection of different data entries.
   2. Information in each can be changed by referencing the index or key and setting that value equal to the new value.
   3. We can iterate through both.
Differences
   1. Objects are referenced based on a number index in arrays. Objects are referenced based on the key in hashes.
   2. Objects stored in hashes are not arranged by a numbered index.
   3. When iterating through hashes and creating do statements, we need to set two parameters(one for the key and one for the value).
   4. Hashes are better for storing items associated with a label. Arrays are better for storing ordered data.
   
# How do you retrieve a particular value from a Hash?

Retrieving data from a hash is similar to that of an array. The main difference is that we use the key in the square brackets, instead of an index number. Let's say we have a hash that represents a person.

  person = {name: "Ryan", occupation: "Comedian"}
  person["occupation"]     #will retrieve the occupation for this person hash.


# How do you add information to a Hash?

Adding data to a hash is similar to that of an array. The main difference is that we use the key in the square brackets, instead of an index number. Let's say we have the same hash from above, but we want to add a "Handiness" category and value rating how handy our person is in tight situations.

  person = {name: "Ryan", occupation: "Comedian"}
  person["handiness"]= "MacGyver"     #will add the handiness for this person hash. 



# How would you perform an operation on every element inside a Hash?

To perform an operationon every element insdie a hash, I would iterate through the hash and create a method to manipulate the value.
Let's say we want to iterate through and print each key-value pair.

  person = {name: "Ryan", occupation: "Comedian"}
  person.each do |key, value|
    puts "#{key}: #{value}"
  end


# How would you change the value of a particular element in a Hash?

A value could be changed the same way that a new value could be added. We would type in the name of the array, followed by the name of the key in square brackets, set equal to the new value. Let's say we want to change our occupation.

  person = {name: "Ryan", occupation: "Comedian"}
  person[:occupation] = "Barista"


# How do you delete an element from a Hash?
We can delete elements from an array by naming the arrary an using the ".delete(:key)" method on the has as seen below:
    person.delete(:occupation)


# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

'nil' will be returned as the value. 


# How do you determine how many elements are in a Hash?

Using the ".length" method on the array name will return the number of key:value pairs.

   person = {name: "Ryan", occupation: "Comedian"}
   person.length # returns 2
