A **key-value collection** (also called a mapping, dictionary, or hash table in different languages) is a data structure that stores pairs of associated values. Each pair consists of a **key** and a **value**. The key is used to look up and retrieve the associated value, similar to how a word in a dictionary is a key that lets you find its definition (the value).

# Key-Value Pairs

The fundamental concept is the key-value pair:

**Key → Value**

For example, in a collection of student information:

* Key: `"Alice"` → Value: `95` (her test score)
* Key: `"Bob"` → Value: `87` (his test score)
* Key: `"Charlie"` → Value: `92` (his test score)

In a collection of city information:

* Key: `"London"` → Value: `8,982,000` (population)
* Key: `"Tokyo"` → Value: `13,960,000` (population)
* Key: `"Paris"` → Value: `2,161,000` (population)

The key is what you use to look up information; the value is what you retrieve.

# Accessing Values

To retrieve a value from a key-value collection, you specify the key, and the collection returns the associated value. This is faster and more intuitive than searching through a list:

```
scores = { "Alice": 95, "Bob": 87, "Charlie": 92 } // Create a key-value collection with some initial pairs
alice_score = scores["Alice"]    // Returns 95
bob_score = scores["Bob"]        // Returns 87
```

# Adding and Modifying Entries

You can add new key-value pairs to a collection or modify existing values. If the key already exists, the value is updated; if the key is new, a new pair is created.

```
scores["David"] = 88              // Add a new pair
scores["Alice"] = 98              // Update an existing value
```

# Constraints on Keys

In most programming languages, keys must be **hashable**—meaning they must be of a type that can be quickly converted to a fixed-size value for fast lookup. Typically, this includes simple types like integers, floats and strings, but not complex types like lists or other collections.

# Use Cases

Key-value collections are extremely useful for any sort of data that is addressed by a unique identifier:

* **Lookups:** Finding information by a natural identifier (like looking up a phone number by name)
* **Configuration:** Storing configuration settings (keys are option names, values are settings)
* **Relationships:** Modeling relationships between entities (like mapping students to their grades)
