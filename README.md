# inflection-js

This repository is based on the [inflection-js](http://code.google.com/p/inflection-js/) repository by [Ryan Schuft](http://www.linkedin.com/in/ryanschuft) hosted on Google Code.

Most of the code, however, was refactored by [Jan Kuča](http://www.linkedin.com/in/jankuca). The new code is structured in one namespace that can be easily used with [Google Closure](http://code.google.com/closure/) Library and Compiler.

    goog.require('string.inflection');

Ryan's original code extends `String.prototype` which is generally considered a bad practice and it might not compile as well as a set of methods in a separated namespace.

## Methods

- string.inflection.**toPlural**(string): string
- string.inflection.**toSingular**(string): string

- string.inflection.**toCamelCase**(string): string
- string.inflection.**toPascalCase**(string): string
- string.inflection.**toTitleCase**(string): string

- string.inflection.**toUnderscored**(string): string
- string.inflection.**toDashed**(string): string
- string.inflection.**toCapitalized**(string): string
- string.inflection.**toHumanized**(string): string

- string.inflection.**toTableName**(string): string
- string.inflection.**toClassName**(string): string
- string.inflection.**toForeignKeyName**(string): string
- string.inflection.**replaceNumbersWithOrdinals**(string): string
