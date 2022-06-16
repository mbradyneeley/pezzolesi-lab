# Pezzolesi Lab

## Making Changes to the Website
* **Adding a new team member**
  * Get a photo from them, open it in apple photos, then click 3 things in this order: edit, crop, square. Save the photo from apple photos to either your local copy of the webpage or the github repository of the webpage. Put it in the folder `pezzolesi-lab/images/teampic`.
  * Open `pezzolesi-lab/_data/team_members.yml` and add a new team member. Follow the format you see in the file EXACTLY with the dash, spaces, tabs, etc. Edit it accordingly including with whatever file type extension your picture is (Of course use their name instead of wherever it says lab member):
  ```
  -name: New Lab Member
   photo: labmember.png
   info: Position in lab
   url: labmemberfirstlastnamenospaces
   group: 1
   ```
   * Now we are going to add their photo and bio to their personal info/overview page. Make a new file for them `pezzolesi-lab/team/newlabmembersname.md`, I would open it side by side with an already existing overview markdown file like `pezzolesi-lab/team/marcuspezzolesi.md` and just copy over everything from Marcus' file and edit it for the new lab member.
   * If you want to remove someone, just do the opposite. Delete their markdown file from the `team/` directory and remove their lines from the `_data/team_members.yml` file. You can leave or delete their image, doesn't really matter if you've done the other two steps.

* **Adding a new publication**
  * Add a photo for your publication to `pezzolesi-lab/images/pubpic`, vertical pictures look better than horizontal. 
  * Like you do when adding a new team member, edit the fields in the file `_data/publist.yml` for the publication.

* **Adding Research**
 * `_pages/research.md`

* **Changing the Home Page**
  * Adding new photos to the slider
  * Editing the Text Fields 

* **Adding to the News Bar on the Homepage**

* **Adding to the Code Page**

* **Adding to the Participation Page**

* **Changing the Contact Page**
