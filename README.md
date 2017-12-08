# Alleys Of Your Mind ver. 2

#### A web landing page that is for the Alleys Of Your Mind radio show.

#### by **Mikey Pinaud**

## Description

This will be a landing page that showcases the Alleys Of Your Mind radio show with logo, past episode images, widgets with audio content, and navigation for upcoming content.

The main inspiration for design comes from this [Spotify](https://open.spotify.com/view/2016-page/) page which there will be a main background image spanning vertically in the background while all content will be floating over as you scroll to the bottom of the page.

## Thoughts and Feedback

After our group decided what the basis of our landing page was about we then started grabbing inspiration for page layout from various google searches using "best CSS sites 2017" or "best CSS layout animation". From that we took ideas from this page and that and started jotting down notes for page layouts, components, and workflow. The next step was to sketch out 2 different wire framing ideas for the layout. We also add main components ideas such as logo, image, and content placement. Starting from desktop and working our way down to tablet and then mobile we started sketching them to different flashcards piece by piece naming each step. For components we also took notes on wish-list items to add if time was given before deadline.

Next step was creating our HTML. We went with the 7-1 SCSS folder layout and started creating all of our partials within. From there is where we learned how to use SASS elements and how to implement them into our workflow. To get a clearer grasp of how to approach SASS we created all of our styling in our main.scss page and then from there we would break them down/"dry our code" by using our 7-1 folder structure using SASS elements and practices.

Is there a better approach to doing this? In time with repetitive practice, especially with knowing how page layout and CSS rules work, will I be able to not have to jot down all the styling on one page and then break them down? Or was the approach we went with common practice?

For me I felt it was a great learning tool implementing various SASS elements from our list one by one honing in on how these would be applied into our workflow. Getting things to work from creating variables, mixins, nesting, and importing seemed easy. Especially since our landing page was pretty minimal.

We has a harder time getting our wishlist components to work as we wanted. Example: Bootstrap Carousel continuous scrolling. Navbar collapsing to the right. Little things like that took mush of our time.

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

## Version 2 Approach

For my approach today I'll be using a lot of the same practices I learned the past couple days. I'll be using more of a 6-1 folder structure for my SASS. There will be all the same assets from Version 1. For this new page layout I would like to implement the grid system from our lesson a few days ago as well as a add a few more content sections.

## Setup/Installation Requirements

[View on web browser](https://mpinaud.github.io/alleys-of-your-mind-version-2/)

Clone or download repository:
  1. Open [this page](https://github.com/mpinaud/alleys-of-your-mind-version-2/) in web browser.
  2. Under the repository name, click Clone or download.
  3. In the Clone with HTTPs section, click to copy the clone URL for the repository.
  4. Open Terminal.
  5. Change the current working directory to the location where you want the cloned directory to be made (ex. cd desktop).
  6. Type git clone, and then paste the URL you copied in Step 3. (ex. git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY).
  7. Press Enter. Your local clone will be created.

## Technologies Used

  * HTML
  * CSS
  * jQuery
  * Bootstrap

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
