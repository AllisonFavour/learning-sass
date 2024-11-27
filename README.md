# SASS
So, i am just getting started with learning SASS which stands for Syntactically Awesome StyleSheets.

I will be following a tutorial by HuXn on YouTube, my approach to learning this will be through coding along with his tutorial video so i can have reference to certain topics when needed later in the future and might also help someone who wants to learn as well. I will also be taking notes of some key concepts or notes to keep in mind.

Firstly, i downloaded cloned his repo for this particular Sass course on github so i can get the image assets he used mainly. Then as you already know, we will be needing a Code editor and a browser, i am using Visual Studio Code (VS Code) as my code editor and Google Chrome and Edge for my browsers to see the output of the stylings.

To get started, i downloaded an extension from VS code, the name of the extension is Live Sass Compiler by Glenn Marks, this is a tool that automatically compiles SASS (SCSS) files into standard CSS files in real-time as you work for the browser to understand. This extention tool makes it much easier to see the changes of your style right away without having to manually run a seperate compiler or having to refresh your browser after each change to your styling code.
Now lets dive into the concepts of SASS

### Variables
Generally in programming, a variable is a container which a value is stored in which anywhere in our program if we need that value we can simply just make a reference to the variable holding that particular value.

How to create a variable in a SCSS file?
Inside our .scss file all we need to do is use the dollar sign followed by the name we want to use for our variable then a colon and the value (in this case the value will be a valid css property).
We can either use a camelCase or name and dash symbol in between the words, here is an example below.
example
$mainColor: #000;
$main-font: 'Roboto', sans-serif;

to use the variable, example below
body {
    background-color: $mainColor;
    font-family: $main-font;
}

In the Variable examples provided above, i used both the camelCase naming convention and the symbol dash in between the words, you can use either of the two for your naming. After creating the Variables i used them as the background-color for the HTML document body and the font-family.

In the Variable folder, we created a project and made use of three variables, $main-color, $bg-image-center, $main-font. The $main-color variable was used to store the color which was used as background-color for our card, the $bg-image-center was use to store the background shorthand properties for centering an image and for the last variable $main-font, it was used to store the Roboto font we imported from Google font using the import keyword in our SCSS file.
Moving onto the next concept, which is Nesting in SASS

### Nesting
Sass allows nesting CSS selectors just like in HTML, 

### Partials
Sass keeps the CSS code DRY (Don't Repeat Yourself). One way to write DRY code is to keep related code in separate files. You can create small files with CSS snippets to include in other Sass files.
Examples of such files can be: reset file, variables, colors, fonts, font-sizes, etc.

The @import directive allows you to include the content of one file in another.


### SASS Mixins
The @mixin directive lets you create CSS code that is to be reused throughout the website.
The @include directive is created to let you use (include) the mixin.
Just like how we have variables in SASS where we can store a single value, the @mixin directive lets us store multiple values to which is to be reused elsewhere in our code, this also helps with the DRY principle which means (Don't Repeat Yourself), so we do not have to repeat bunch of styling code over and over again.
To create a mixin we make use of the @ symbol follow by the mixin keyword and then we give it a name which it can be referenced with, the naming must either follow the camelCase naming convention or multiple-words-spaced-out with dash.
Then to use the mixin we have to use the @include directive, we write the @include directive followed by the name we used in creating the mixin.


### Extends
The SASS @extend directive lets you share a set of CSS properties from one selector to another.
The @extend directive is useful if you have almost identically styled elements that only differ in some small details.


### SASS Operators
Operator is a symbol that tells the compiler to perform specific mathematical, conditional or logical functions. It is a symbol that operates on a value or a variable.
The equality operators return whether or not two values are the same.
eqaul to ==
not equal to !=
Boolean refers to a value that is either true or false.
Equality Operators
(and) if both conditions are true then the value will be true, otherwise false
(or) if either conditions are true then the value will be true, otherwise false
(not) returns the opposite value
Relational Operators
< less than
> greater than
<= less than or equal to
>= greater than or equal to



### SASS Functions
Functions allow you to define complex operations on SassScript values that you can re-use throughout your stylesheet.
They make it easy to abstract out common formulas and behaviors in a readable way.



### Interpolation
Interpolation can be used almost anywhere in a Sass stylesheet to embed the result of a SassScript expression into a chunk of CSS. Just wrap an expression in pound sign symbol followed by curly braces #{}



### Directive
Condtional statement: this are a steps or rules that allow us to control the flow of our program.
@if
@else if
@else
for loop
each loop
while loop



### Portfolio Project
3:31:58