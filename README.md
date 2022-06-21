# Pezzolesi Lab

## Making Changes to the Website
* **Adding a new team member**
  * Get a photo from them, open it in apple photos, then click 3 things in this order: edit, crop, square. Save the photo from apple photos to either your local copy of the webpage or the github repository of the webpage. Put it in the folder `pezzolesi-lab/images/teampic`.
  * Open `pezzolesi-lab/_data/team_members.yml` and add a new team member. Follow the format you see in the file EXACTLY as seen, with the dash, spaces, tabs, etc (**THIS IS THE PRACTICE YOU SHOULD USE THROUGHOUT YOUR UPDATES OF THE WEBPAGE**). Edit it accordingly including with whatever file type extension your picture is (Of course use their name instead of wherever it says lab member):
  ```
  -name: New Lab Member
   photo: labmember.png
   info: Position in lab
   url: labmemberfirstlastnamenospaces
   group: 1
   ```
   * Now we are going to add their photo and bio to their personal info/overview page. Make a new file for them `pezzolesi-lab/team/newlabmembersname.md`, I would open it side by side with an already existing overview markdown file like `pezzolesi-lab/team/marcuspezzolesi.md` and just copy over everything from Marcus' file and edit it for the new lab member.
   * If you want to remove someone, just do the opposite. Delete their markdown file from the `team/` directory and remove their lines from the `_data/team_members.yml` file. You can leave or delete their image, doesn't really matter if you've done the other two steps.
   * Adding someone as alumni: Simply put their group number as 8 instead of 1.

* **Adding a new publication**
  * Add a photo for your publication to `pezzolesi-lab/images/pubpic`, vertical pictures look better than horizontal. 
  * Like you do when adding a new team member, edit the fields in the file `_data/publist.yml` for the publication.

* **Adding Research**
 * Open the file `_pages/research.md` and create a new section based off of the other research files. Place text between the <div></div> tags. If you want to add links to any of the text such as links to papers, etc do this: \[So and so's paper, et. al.](https://link-to-paper-here-in-parenthesis.com). To add an image, look for this above the text block and change the file to your image which you should put in the `images/respic` folder: <br/>
\![]({{ site.url }}{{ site.baseurl }}/images/respic/scn2aMut.png){: style="width: 300px; float: left;margin-right: 30px; border: 10px"}


* **Changing the Home Page**
  * Changing photos on the slider
    * This one is a little trickier especially if you are adding or removing images because that requires some extra changes. Open up `_pages/home.md` and you should see some html with the word carousel and then some markdown text below the html block. In the html block, you'll see a list of items and each item has a path to an image. Make sure your image has been cropped with apple photos to a 3:2 aspect ratio, save it to the foler `images/slider7001400`. The images show in order of how the list is ordered, so replace an image wherever in the list that you would like your image to be. If you want to add it as an additional image instead of replacing another, copy the three lines making up an item of the list, make it the next numbered slide (if there are 5 current slides, make it 'Slide 6') and add your photo's filename to it. Then at the top of the html block you'll see carousel indicators, add a new data slide row to that, incrementing your new slide's number (for slide 6 you would make data-slide-to="5" because they start at 0).

  * Editing the Text Fields 
    * Below the html block in the file `_pages/home.md`, you can write whatever you like, easily renaming, adding or changing sections. It is all in github markdown syntax which is easily learned and there are plenty of guides on the internet. A new heading is made like so: \###My Research. Then hit 'enter', start a new line and type away. Adding \<br/> where you want a break in a line or a new line will be helpful here or in markdown in general.

* **Adding to the News Bar on the Homepage**
  * This is easy. Open up the file `_data/news.yml` and copy what is already there. Add a date and a headline using the exact same formatting as the rest of the file. If you want to add a link from some text to a webpage add this in the middle of your sentence in the headline: \<a href='https://your-link.com'>Whatever you type right here will be blue and linked to the link you provided</a>. Unfortunately, adding videos is pretty tricky, if you want to do that, you can try and replicate what I did for the 15 July, 2019 news headline. I made the photo thumbnail, and added it to images and the rest was tricky html which you can see in that news headline.

* **Adding to the Code Page**
  * This one is changed by accessing the file `_pages/code.md`. You can add a link to the source code on github by making a link like done in the 'Adding Research' section with the \[title](website) syntax. You can add an image on the next line, add it to the `images/codepic` folder and then change the name of the existing file to your pictures name. You can add information about your code/project on the next line, and the last line is an explicit link to the github repo with a nice little github icon. If adding more to this page, I would copy the lines from the project we have on there currently and place the next project below. You should have 3 dashes between each project as well as 3 dashes above the first and below the last project like so: <br/>
\---<br/>
proj1<br/>
\---<br/>
proj2<br/>
\---<br/>

* **Adding to the Participation Page**
  * Currently empty, open for formatting as you like. You can copy the format from another file/page that you are comfortable with and place it in here `_pages/participation.md`.

* **Changing the Contact Page**
  * This one is all in markdown, see the info on editing the homepage for some basics on markdown, googling markdown is great for help too. You can just edit the text here however you want. Adding \<br/> where you want a break in a line or a new line will be helpful here or in markdown in general. This file is found here: `_pages/contact.md`.
