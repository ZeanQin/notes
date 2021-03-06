<!-- TITLE: Hashing -->
<!-- SUBTITLE: A quick summary of Hashing -->

# What is Hashing
A hash is like a fingerprint for data. A hash function takes your data — which can be any length — as an input, and gives you back an identifier of a smaller (usually), fixed (usually) length, which you can use to index or compare or identify the data.

> **Intuition**: a hash function builds a (sometimes not strict, i.e. collision) one-to-one relationship between a piece of data and a number
{.is-success}

A sample hash can be: 

`b3f9b3a3504ccb29c4183730a42c8d56`

# Properties of Hash Functions
* The same input always hash to the same identifier
* Most hash functions are one-way operations, which is to say you can figure out an identifier from the data, but you typically can’t do the reverse.
* Ideally, the output values should be distributed uniformly — that is, each possible output should be equally likely
* For a lot of use-cases it is also important that the outputs be distributed randomly; similar inputs should not give similar outputs.
* For some use-cases — usually in security — it is also important to minimise collisions, meaning, as far as possible, each input should give a unique output.
* Finally, in most cases (though not always), you want it to be fast.

# Common Hashing Algorithms
There are literally thousands of named hashing functions. Some are secure, but comparatively slow to calculate. Some are very fast, but have more collisions. Some are close to perfectly uniformly distributed, but very hard to implement. You get the idea. If there’s one rule in programming it’s this: there will always be trade-offs.

* SHA-1 — Secure Hash Algorithm — was devised by the NSA, and for a long time was used to secure lots of Internet communication.
* MD5 is another popular one, often used to prove that the file you’re downloading is the one you think it is. 
* CityHash
* MurmurHash
* SpookyHash
# Related Links
* https://blog.medium.com/what-are-bloom-filters-1ec2a50c68ff

