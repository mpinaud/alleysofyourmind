# Alleys Of Your Mind ver. 2

A web landing page that is for the Alleys Of Your Mind radio show. This process was to learn SASS while focusing on responsive UI design.

![alt text](https://github.com/mpinaud/alleys-of-your-mind-version-2/blob/master/img/logo/aoym-logo.png)

[View on web browser](https://mpinaud.github.io/alleys-of-your-mind-version-2/)

# What I Learned

* SASS

## Elements Used

<table>
  <thead>
    <tr>
      <th>SASS Element</th>
      <th>DESCRIPTION</th>
      <th>IMPLEMENTATION</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Variables</td>
      <td>Allow you to define a value once and use it in multiple places. Variables begin with dollar signs and are set like CSS properties. You can change the value of the variable in one place, and all instances where it is used will be changed, too.</td>
      <td>Within our Abstracts folder we have placed a file called variables in which here is where we created variables for our media query sizes, background colors and width styling, borders height and alignment styling, and for z-indexing. Individual variables where then called in various pages in our SCSS directory</td>
    </tr>
    <tr>
      <td>Mixins</td>
      <td>Lets you make groups of CSS declarations that you want to reuse throughout your site. You can even pass in values to make your mixin more flexible.</td>
      <td>Within our Abstracts folder we have placed a file called variables in which here we created a single mixin called flex-center in which we declared a value of display flex and justify content center where we were able to call in our main.scss page for our grid system. To call this CSS declaration we had to start it with @include followed by the mixins name which was flex-center.</td>
    </tr>
    <tr>
      <td>Partials</td>
      <td>Files that contain little snippets of CSS that you can include in other Sass files. This is a great way to modularize your CSS and help keep things easier to maintain. A partial is simply a Sass file named with a leading underscore. Sass partials are then used with the @import directive.</td>
      <td>Within the SCSS directory we have our main folders which within those we have created partials. This makes modularizing sections of our code easier and faster to go through if needed to do any changes. Example: Our layout folder we created various partials for our page layout. navigation.scss was created so if we needed to make any changes to our navbar this makes it clearer and easier to find rather than scrolling through a single page of CSS to find the navbar section</td>
    </tr>
    <tr>
      <td>Nesting</td>
      <td>Lets you nest your CSS selectors in a way that follows the same visual hierarchy of your HTML.</td>
      <td>Within our layout folder we have a partial called header.scss. For our styling of .header we have nested a media query calling our mobile variable and changing it's height.</td>
    </tr>
    <tr>
      <td>Import</td>
      <td>Lets you split your CSS into smaller, more maintainable portions. Sass will take the file that you want to import and combine it with the file you're importing into so you can serve a single CSS file to the web browser.</td>
      <td>Within each of our SCSS subfolders we've created a modules.scss partial which has imported each of the other partials in that folder. Example: Our modules.scss partial in our layout folder is importing all of our other partials in the layout folder. I use this we must use @import and then in quotes you call each partial without having to add the underscore or the .scss.</td>
    </tr>
  </tbody>
</table>

## Technologies Used

  * HTML
  * CSS
  * SASS
  * Bootstrap v3.7.7
  * jQuery

## License

Copyright (c) 2017 Mikey Pinaud

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
