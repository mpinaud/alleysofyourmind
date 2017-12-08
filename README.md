# Alleys Of Your Mind ver. 2

#### A web landing page that is for the Alleys Of Your Mind radio show.

#### by **Mikey Pinaud**

## Description

This will be a landing page that showcases the Alleys Of Your Mind radio show with a logo, past episode images and widgets of which you can listen to past show and navigation for upcoming content.

The main inspiration for design comes from this [Spotify](https://open.spotify.com/view/2016-page/) page which there will be a main background image spanning vertically in the background while all content will be floating over as you scroll to the bottom of the page.

## Thoughts and Feedback


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
      <td>Mixin</td>
      <td>Lets you make groups of CSS declarations that you want to reuse throughout your site. You can even pass in values to make your mixin more flexible.</td>
      <td>Within our Abstracts folder we have placed a file called variables in which here we created a single mixin called flex-center in which we declared a value of display flex and justify content center in which we were able to call in our main.scss page for our grid system. To call this CSS declaration we had to start it with @include followed by the mixin name which was flex-center.</td>
    </tr>
    <tr>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
    <tr>
      <td> </td>
      <td> </td>
      <td> </td>
    </tr>
  </tbody>
</table>

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
