This is a 20 minute prototype of a new language idea for a system of laws/government that is: human readable, mathematically minimal, and strongly typed language.

I am posting in response to: https://news.ycombinator.com/item?id=19993720

You can [try the language Jefferson in the Tree Language builder](http://treenotation.org/sandbox/build/#grammar%0A%20nodeType%20jefferson%0A%20%20root%0A%20%20description%20A%20prototype%20language%20for%20a%20human%20readable%2C%20mathematically%20minimal%2C%20strongly%20typed%20language%20for%20writing%20laws%2Fgovernments%2Fconstitutions.%0A%20%20catchAllNodeType%20errorNode%0A%20%20inScope%20preamble%20article%0A%20cellType%20englishWord%0A%20%20highlightScope%20string%0A%20cellType%20int%0A%20%20highlightScope%20constant.numeric.integer%0A%20cellType%20organizationName%0A%20%20highlightScope%20entity.name.label%0A%20cellType%20parentOrganizationName%0A%20cellType%20personName%0A%20cellType%20powerName%0A%20cellType%20keywordCell%0A%20%20highlightScope%20keyword%0A%20cellType%20state%0A%20cellType%20president%0A%20%20extends%20personName%0A%20cellType%20senatorName%0A%20%20extends%20personName%0A%20nodeType%20keyword%0A%20%20firstCellType%20keywordCell%0A%20%20abstract%0A%20nodeType%20clause%0A%20%20abstract%0A%20%20extends%20keyword%0A%20nodeType%20article%0A%20%20inScope%20section%0A%20%20cells%20int%0A%20%20extends%20keyword%0A%20nodeType%20assignmentOfPower%0A%20%20cells%20organizationName%20powerName%0A%20%20match%20assignPowerTo%0A%20%20extends%20clause%0A%20nodeType%20description%0A%20%20description%20English%20description%20of%20entity.%0A%20%20catchAllCellType%20englishWord%0A%20%20extends%20keyword%0A%20nodeType%20errorNode%0A%20nodeType%20newOrganization%0A%20%20description%20A%20clause%20establishing%20a%20new%20organization%0A%20%20cells%20organizationName%0A%20%20catchAllCellType%20parentOrganizationName%0A%20%20extends%20clause%0A%20nodeType%20newPower%0A%20%20cells%20powerName%0A%20%20inScope%20description%0A%20%20extends%20clause%0A%20nodeType%20preamble%0A%20%20catchAllCellType%20englishWord%0A%20%20extends%20keyword%0A%20nodeType%20section%0A%20%20inScope%20clause%0A%20%20cells%20int%0A%20%20extends%20keyword%0Asample%0A%20preamble%20We%20the%20People%20of%20the%20United%20States%2C%20in%20Order%20to%20form%20a%20more%20perfect%20Union%2C%20establish%20Justice%2C%20insure%20domestic%20Tranquility%2C%20provide%20for%20the%20common%20defence%2C%20promote%20the%20general%20Welfare%2C%20and%20secure%20the%20Blessings%20of%20Liberty%20to%20ourselves%20and%20our%20Posterity%2C%20do%20ordain%20and%20establish%20this%20Constitution%20for%20the%20United%20States%20of%20America.%0A%20article%201%0A%20%20section%201%0A%20%20%20newOrganization%20Congress%0A%20%20%20newOrganization%20Senate%20Congress%0A%20%20%20newOrganization%20House%20Congress%0A%20%20%20newPower%20legislative%0A%20%20%20assignPowerTo%20Congress%20legislative)

The benefits of this language are:

- complexity can be measured. in our present system of government, complexity is the weapon of special interests. With this language system, two "laws/patches" can be easily measured and it can be unjustifiable to pass the more complex version.
- clean code. every character counts and every line is version controlled. laws are easy to compute with.
- as little ambiguity as possible.

Instructions:

The language is called "jefferson" is defined in "jefferson.grammar" and the beginning of the US Constitution is written in this language in "constitution.jefferson".

If you put it in the Tree Notation console you get syntax highlighting and type checking. You can also install jtree "npm install -g jtree", and then generate syntax highlighting for Sublime, et cetera.


