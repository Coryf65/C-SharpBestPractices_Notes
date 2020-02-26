# C# Best Practices for Developers
[Linkedin](https://www.linkedin.com/learning/c-sharp-best-practices-for-developers/what-you-should-know-before-watching)


## What are Best Practices

### Naming and Handling Classes
  - Namespace : Company.ProgramLayer
* Class Naming
  - Classes = PascalCase, Nouns
  - Methods = PascalCase, Verbs
  - Fields = camelCase, Private
  - Properties = PascalCase, at start
* Access Modifiers
  - Keeps all in Private, unless you are desinging otherwise
* Avoid 
  -Prefixes, Underscores, abbreviations
  
### Constructors
*(method of a class that gets created on intialization)*
  
  * Provide a Default Constructor
  * Consider paramaterized constructors
  * Name the parameters the same as related properties
  
  * Avoid - Don't make them do too much work, Simple is key

### Namespaces
*organizes classes in a heirarchy*

  * Follow Format: 
      - [Comany].[Technology].[Feature]
      - *example Microsoft.Media.Design*
  * PascalCasing
  * use the import/using instead of calling directly to a function
  
  * Avoid naming the Namespace the same as the class

### Staic Classes
*a static class cannot be instantiated, good for services (logging, notifications)*

  * Use sparingly
  * use for common utilites
  
  * Avoid as a random bucket


#### Test Driven Development Notes

1. Arrange (create the test expectations)
2. Act     (run the desired test / method)
3. Assert  (Run the test against the expected and the actual)
