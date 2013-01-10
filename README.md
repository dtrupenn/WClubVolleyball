# Women's Club Volleyball Site

This is the source material for the Women's Club Volleyball team includes some scripts for a picture viewer for images and a script that gets facebook profile pics based on their usernames.

## Resources for the Uninitiated
* http://twitter.github.com/bootstrap/
* http://www.w3schools.com/html/default.asp
* http://www.w3schools.com/css/default.asp
* http://www.w3schools.com/js/default.asp (Probs don't need it, but is slightly used)


## Adding/Removing photos to Gallery
In order add an image you must modify the media.html file and add your desired jpg image to the images folder (try to keep the image around the same size as the ones already there to keep it from looking fugly).

In the media.html file go to line 71 of the code where you will find a huge list of images listed under the div called myCarousel. In order to add any images to this you must go inside the carousel-inner div starting at line 73 and add these lines of code at the end of the list of images for EACH image:

    <div class="item">
      <img src="images/[filename].jpg" alt="">
    </div>

To remove simply remove the div block (like the one specified above) from the list for your specified image.

## Adding/Removing Team Members
In order to add a Team Member you must modify the team.html file and add your desired player jpg image to the images folder(try to keep the images about the same size as the ones there or at least the same width as the current ones, to keep it looking nice).

In the team.html file go to line 92 of the code where you will find a huge table of your team members. Each row in the table is defined by the <tr></tr> tag so to add a new team member simply add the following code to the list of members:

    <tr>
      <!-- Team member name -->
      <td>
        <img src="images/[filename].jpg"/>
      </td>
      <td>
        <p>Name: [Name]</p>
        <p>Year: [Year]</p>
        <p>School: [SEAS/SAS/Nursing/Wharton]</p>
        <p>Position: [Position]</p>
        <p>Height: [feet]'[inches]"</p>
        <p>Hometown: [Location]</p>
      </td>
    </tr>

To remove simply remove the tr block (like the one above) from the list for the existing team member.
