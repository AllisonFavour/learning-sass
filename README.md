# Sass
So, i am just getting started with learning SASS which stands for Syntactically Awesome StyleSheets.

I will be following a tutorial by HuXn on YouTube, my approach to learning this will be through coding along with his tutorial video so i can have reference to certain topics when needed later in the future and might also help someone who wants to learn as well. I will also be taking notes of some key concepts or notes to keep in mind.

Firstly, i downloaded cloned his repo for this particular Sass course on github so i can get the image assets he used mainly. Then as you already know, we will be needing a Code editor and a browser, i am using Visual Studio Code (VS Code) as my code editor and Google Chrome and Edge for my browsers to see the output of the stylings.

To get started, i downloaded an extension from VS code, the name of the extension is Live Sass Compiler by Glenn Marks, this is a tool that automatically compiles SASS (SCSS) files into standard CSS files in real-time as you work for the browser to understand. This extention tool makes it much easier to see the changes of your style right away without having to manually run a seperate compiler or having to refresh your browser after each change to your styling code.
Now lets dive into the concepts of SASS

## Variables
Generally in programming, a variable is a container which a value is stored in which anywhere in our program if we need that value we can simply just make a reference to the variable holding that particular value.
How to create a variable in a SCSS file
inside our .scss file all we need to do is use the dollar sign followed by the name we want to use for our variable then a colon and the value (in this case the value will be a valid css property).
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

## Nesting
