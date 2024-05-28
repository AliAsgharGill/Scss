**We can declare the following in scss.**

**1. Variables with $ e.g => $bg-color: red, $secondary-color: #000**

**Nesting Guide**
    *2. Nesting with  & in the parent element, class, or id.  we can > h1 for direct child, mean h1 child of div or any other parent element in brackets but direct name only h1 will also be applied at children also.*

**3. Operators We can also use operators +, -, *, /.**

**4. @mixin, it is a simple function that have some properties and we can call them with ( @include functionName ) again and again.**
    *We can also use parameters in this function, e.g @include functionName(param1:default Parameter here, param2: default Parameter here){} and then can call it like @include functionName(red, 1rem), if we forgot to give parameter while calling function then it give error, but if default parameter exist then no error.*
    *4.1 we can also make a template using  percentage %, e,g %custom{} but it not accept parameters so we can use @mixin instead of it.*

**5. Partials(patches, different files for each type of code ),  we can make partial files for different code, like one partials for $variables other for @mixins etc.**

**6. @extend, (inheritance) with this keyword we can use properties of another element, class, id.**

**Import and Use Guide**
*NOTE=> start file name with underscore so use compiler will not compile it, so no need to compile it. e.g  _variables.scss, _mixins.scss etc, and then need to import that file in main.scss or any other root scss file by using @import "fileName" without .scss and underscore, these both are optional. if there is two file with same name which have different shades of colors or other properties it get override because of same name of file, so we need to Use (@use fileName instead of @import) and then can use like @use "fileName" as "anyName"*
