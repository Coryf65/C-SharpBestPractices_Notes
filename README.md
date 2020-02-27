# C# Best Practices for Developers
[Linkedin](https://www.linkedin.com/learning/c-sharp-best-practices-for-developers/what-you-should-know-before-watching)

more Resources
[w3 Schools](https://www.w3schools.com/)

[Microsoft Docs](https://docs.microsoft.com/en-us/dotnet/csharp/)

[Stack Overflow](https://stackoverflow.com/)


## What are Best Practices

* D.R.Y
* K.I.S.S
* Always, Always check for Null
* when possible use a USING() statement

### Naming and Handling Classes
  - Namespace : Company.ProgramLayer
* Class Naming
  - Classes = PascalCase, Nouns
  - Constuctors
  - Methods = PascalCase, Verbs  
  - Fields = camelCase, Private
  - Properties = PascalCase, at start
  - Constants = PascalCase
  - Vars = camelCase
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

### Singletons

  * Use when you only need one instance
  * Use when you need to create 'child objects'
  * Use to Support OOP features
  
  * Avoid if you won't leverage any of the aforementioned features

### Method Overloading

  * Include comments for the methd and parameters (xml for intellisense)
  * Use few Parameters
  * Order the parameters consistently
  
  * Avoid overloads with the same name but different purpose, and duplicate Code
  
### Method chaining
*when one method calls another method to get most of the work done*
  
  * Implement to reduce repeated code
  
  * Avoid if it's overkill and will overcomplicate things

### Constants vs. Read-only fields

  #### Constants
  * PascalCasing
  * Compile-time constant
  * assigned on declaration
  * only number, boolean or string
  * Always Static
  
  #### Read-Only
  * PascalCasing
  * Runtime constant
  * assigned on declaration or constructor
  * any data type
  * optionally static

### Property
*flexible mechanism that allows you to, Read, Write Compute it's value on a Private Field* 

  * Lazy-Loading
  * Validate incoming values
  * Use Relevant Names
  * use 'getter' for simple protection, formatting and initilalizing
  * use 'setter' for simple protection, formatting and validation
  
  * Avoid abbreviation, complex logic
  
#### Test Driven Development Notes

1. Arrange (create the test expectations)
2. Act     (run the desired test / method)
3. Assert  (Run the test against the expected and the actual)
