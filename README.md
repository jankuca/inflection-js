**_This repository just a fork from [http://code.google.com/p/inflection-js/](http://code.google.com/p/inflection-js/)_**


This project is a port of the functionality from Ruby on Rails' Active Support Inflection classes into Javascript. 
Instead of supporting the functionality in a new Inflector object, I've chosen to extend the Javascript String object. 

This was ported initially to support plurality in Jester (http://thoughtbot.com/projects/jester). 

If anyone requires a different license in order to use this, please let me know and I can switch it over.
I intend for this to be generally available for anyone's usage, and am not intentionally limiting it.

_Currently supported:_

```javascript

String.pluralize(plural) == String
  //renders a singular English language noun into its plural form
  //normal results can be overridden by passing in an alternative

String.singularize(singular) == String
  //renders a plural English language noun into its singular form
  //normal results can be overridden by passing in an alterative

String.camelize(lowFirstLetter) == String
  //renders a lower case underscored word into camel case
  //the first letter of the result will be upper case unless you pass true
  //also translates "/" into "::" (underscore does the opposite)

String.underscore() == String
  //renders a camel cased word into words seperated by underscores
  //also translates "::" back into "/" (camelize does the opposite)

String.humanize(lowFirstLetter) == String
  //renders a lower case and underscored word into human readable form
  //defaults to making the first letter capitalized unless you pass true

String.capitalize() == String
  //renders all characters to lower case and then makes the first upper

String.dasherize() == String
  //renders all underbars and spaces as dashes

String.titleize() == String
  //renders words into title casing (as for book titles)

String.demodulize() == String
  //renders class names that are prepended by modules into just the class

String.tableize() == String
  //renders camel cased singular words into their underscored plural form

String.classify() == String
  //renders an underscored plural word into its camel cased singular form

String.foreign_key(dropIdUbar) == String
  //renders a class name (camel cased singular noun) into a foreign key
  //defaults to seperating the class from the id with an underbar unless
  //you pass true

String.ordinalize() == String
  //renders all numbers found in the string into their sequence like "22nd"
      
```
  
Thanks,

Ryan Schuft (ryan.schuft@gmail.com)
