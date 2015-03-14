Some type class instances can be automatically derived from the structure of types. As a result, the Haskell language includes the "deriving" mechanism to automatic generates such instances for a small number of built-in type classes. RepLib is a GHC library that enables a similar mechanism for arbitrary type classes. Users of RepLib can define the relationship between the structure of a datatype and the associated instance declaration by a normal Haskell functions that pattern-matches a representation types. Furthermore, operations defined in this manner are extensible---instances for specific types not defined by type structure may also be incorporated.