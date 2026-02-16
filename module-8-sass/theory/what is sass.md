# what is sass ?

Sass is a CSS preprocessor that extends the capabilities of regular CSS by introducing features like variables, nesting, mixins, and functions.

It allows developers to write more maintainable and efficient stylesheets by providing a more structured and organized way to manage CSS code.

Sass files typically have the extension `.scss` or `.sass`, and they are compiled into standard CSS before being used in web projects.

This makes it easier to create complex stylesheets while keeping the code clean and reusable.

Sass also supports features like inheritance, which allows you to share styles between selectors, and it provides a powerful set of built-in functions for manipulating colors, strings, and other values.


Overall, Sass is a popular tool among web developers for enhancing the capabilities of CSS and improving the workflow of styling web applications.


**advantage of sass**

1. **Variables**: Sass allows you to use variables to store values such as colors, fonts, or any CSS value. This makes it easier to maintain and update styles across your project.

2. **Nesting**: Sass supports nesting of selectors, which helps to organize your CSS in a more hierarchical and readable way. This can reduce the amount of code you need to write and make it easier to understand the structure of your styles.

3. **Mixins**: Mixins are reusable blocks of code that can be included in other selectors. This allows you to avoid repetition and keep your styles DRY (Don't Repeat Yourself).

4. **Functions**: Sass provides built-in functions for manipulating colors, strings, and other values. You can also create your own custom functions to perform specific tasks.

5. **Partials and Imports**: Sass allows you to break your stylesheets into smaller, more manageable files called partials. You can then import these partials into a main stylesheet, which helps to keep your code organized.

6. **Inheritance**: Sass supports inheritance through the use of the `@extend` directive, which allows you to share styles between selectors without duplicating code.

Overall, Sass enhances the capabilities of CSS and provides a more efficient and maintainable way to write stylesheets for web development projects.


## how to install sass ?

To install Sass, you can use npm (Node Package Manager) if you have Node.js installed on your system. Here are the steps to install Sass:

1. Open your terminal or command prompt.
2. Run the following command to install Sass globally:

   ```
   npm install -g sass
   or
   npm install sass --save-dev

   ```

This will allow you to use the `sass` command from anywhere in your terminal.

After installation, you can verify that Sass is installed correctly by running:

```sass --version
```

This should display the version of Sass that you have installed.

Once you have Sass installed, you can compile your `.scss` or `.sass` files into standard CSS using the command line. For example:

```sass input.scss output.css
```

This command will take your `input.scss` file and compile it into `output.css`, which you can then include in your web project.

Alternatively, you can set up a watch command to automatically compile your Sass files whenever they change:

```sass --watch input.scss:output.css
```

This will keep an eye on your `input.scss` file and automatically update `output.css` whenever you make changes to the Sass file.

You can also use build tools like Webpack, Gulp, or Grunt to automate the Sass compilation process as part of your development workflow.
Overall, installing Sass is straightforward, and it provides a powerful way to enhance your CSS development process.



## variables in sass 

   **A variable ids used to stored an information of data there we used variable**

   1. in sass variables is used to stored color | background color | size | margin | fonts etc.

   2. we used a variables to stored with $ symbol

   **examples**

```
  $bg-violet:#764199;
  $txt-violet:#764199;
  $bg-pink:#f3a6cc;
  $txt-pink:#f3a6cc;
  $bg-white:white;
  $txt-white:white;
  $max-width:100%;
  $min-width:80%;
  $max-height:auto;
  $min-height:auto;

 // main stylesheet
 #header
 {
 width: $max-width;
 height: auto;
 display: flex;
 flex-wrap: wrap;   
 }
 .logo
 {
 width: 55%;
 height: auto;
 margin: 3px;
 padding: 8px;   
 }
 .logo img 
 {
 width: 20%;   
 }

 .navbar
 {
 width: 40%;
 height: auto;
 margin: 3px;
 padding: 8px;   
 }
 .navbar ul li 
 {
 display: inline-block;
 padding: 8px 15px;
 text-decoration: none;
 list-style-type: none;

 }
 .navbar a 
  {
  text-decoration: none;
  list-style-type: none;  
  color: black;
  font-size: 20px;
  }
  #reg 
  {
 width: auto;
 height: auto;
 padding: 8px;
 border: 0;
 background-color: $bg-violet;   
 color: $txt-white;
 border-radius: 2px;
 }
 #hero-section 
 {
 width: $max-width;
 height: auto;
 display: flex;
 flex-wrap: wrap;    
 }
 .banner-txt
 {
 width: 45%;
 height: auto;
 padding: 25px;    
 }
 .banner-txt h1 
 {
    color: #764199;
    font-size: 58px;
 }
 #para
 {
    color: #f3a6cc;
 }

 .banner-img
 {
 width: 45%;
 height: auto;
 padding: 25px;    
 }
 .banner-img img 
 {
    width: 70%;
    height: auto;
  }
 ``` 
 
## nesting in sass

 **nesting sass**
 Sass supports nesting of selectors, which helps to organize your CSS in a more hierarchical and readable way. This can reduce the amount of code you need to write and make it easier to understand the structure of your styles.

 **examples**

 ```
     .menu 
    {
        width: auto;
        height: auto;
        li 
        {
            display: inline-block;
            padding: 5px 25px;
            text-decoration: none;
            list-style-type: none;

           a{
             text-decoration: none;
            list-style-type: none;
            color: white;
           } 
        }
    } 

}
 ```

## what is sass mixin ?
  **definition**
  1. sass mixin is used to re-usables code
  2. sass mixin basically used for re-used style one section to another section 
  3. A mixin is define once and include anywhere in your stylesheet
  4. A mixin is help you to avoid repeattion of code.
  5. A mixin is used to keep code clean and write dynamic styles using parameters and conditions and logic.

  **syntax of mixing**

  ```
  @mixin mixin-name {
   re-usables of code 
  }

  @include mixin-name
  
  ```   


 







