# [RecipeShare](https://share-recipe-aaron.herokuapp.com/)

## Contents
1. [Summary](#summary)
1. [UX](#ux)
    1. [Strategy](#strategy)
    1. [Scope](#scope)
    1. [Structure](#structure)
    1. [Skeleton](#skeleton)
    1. [Surface](#surface)
1. [Features](#features)
    1. [Existing Features](#existing-features)
    1. [Features left to implement](#left-to)
1. [Bugs](#bugs)
1. [Technologies used](#tech)
1. [Testing](#testing)
1. [Deployment](#deployment)
    1. [Github Pages](#github)
    1. [heroku](#heroku)
1. [Credits](#credits)
    1. [Content](#content)
    1. [Acknowledgements](#acks)

# <a name="summary"></a> Summary
This site is a virtual cookbook.

It provides a database of recipes which can be searched, viewed, added to, removed from and edited.

# <a name="ux"></a> UX
## <a name="Strategy"></a> Strategy
### **New site user's goals:**
* As a new site user, I want to be able to browse and search for recipes 
* As a new site user, I want to get inspiration for a recipe to make
* As a new site user, I want to be able to understand the intent of the page
* As a new site user, I want I want to understand easily how to navigate the page and access the facilities provided
### **Returning user's goals**
* As a returning site user, I want to be able to log in
* As a returning site user, I want to be able to view my recipes
* As a returning site user, I want to be able to edit and delete my recipes
* As a returning site user, I want to be able to add new recipes
### **Site owner'as goals:**
* As a site owner, I want recipes added via the site to be stored in the correct format in the database
* As a site owner, I want to be able to see who has added each recipe

## <a name="scope"></a> Scope
**Functional requirements:**
#### For ease of use:
* Navigation bar which is simple and easy to navigate
* A search Function
#### To ensure the database is up to date and editable:
* Function to add a recipe
* Function to edit a recipe
* Function to delete a recipe
* For the recipes to be only editable by the creator

**Content requirements:**
#### To ensure the site is visually appealing and to draw the user's eye:
* A background image which would be pleasing to have througout the site.
* Clear, crisp colours which do not detract from or make the text unreadable

### For usability
* For the time commitment to be clear as this is often a factor in a recipe choice

## <a name="structure"></a> Structure
**Interaction design:**
* User friendly interface to ensure usability and to encourage the user to return
* Responsive and visible links which change on hover to provide user feedback as they navigate the site
* Ability to exit pop ups so a user is not forced to use the browser navigation tools

**Information Architecture:**
* Navigation bar at the top of the page
* Responsive navigation bar - adjusting for mobile for ease of use
* All features appropriate size and responsive for mobile and desktop viewing
* All information is appropriate and relative to the subject and not misleading or hard to find

## <a name="skeleton"></a> Skeleton
Please click the below link to view the wireframe mock up of the website in mobile, tablet and desktop sizing

[Wireframe](https://github.com/AaronHughes424/ShareYourRecipe/tree/main/static/wireframes)

## <a name="surface"></a> Surface
The intention of the website is to be clean, crisp and clear

* The colour scheme selected is shades of orange and white.
* The colour scheme was selected as it is clean and crisp. It's bright colours make usability fun.

# <a name="features"></a> Features
## <a name="existing-features"></a> Existing Features
Feature | Details
--------|--------
Log in | The user can register and log into their own account with personalised features
Log out | There is a log out functionality on the page - this is especially important for users of a shared device
Add recipe | Users can contribute to the site via the add recipe form
Edit recipe form | Users are able to edit their own recipes. An important note here is that users can only edit their own recipes
Delete a recipe | Users are abel to delete their own recipes. As above, this can only be done with the user's own recipes
Search function | The users are able to search the recipe database by ingredient and recipe name.

# <a name="bugs"></a> Bugs
Bug | Fix
--------|--------

* Issue with heroku deployment|When posting the MongoDB URI from the env.py file there was a line break which wouldn't allow heroku to launch app.

# <a name="tech"></a> Technologies Used
* Materialize - https://materializecss.com/
* JavaScript
* www.validator.w3.org
* http://www.css-validator.org/
* Git
* Gitpod
* GitHub
* Google Chrome
* http://www.responsinator.com/
* Chrome Dev Tools
* Python
* Flask
* MongoDb
* Heroku
* Jinja
* Balsamiq

# <a name="testing"></a> Testing
### **New site user testing:**
* As a new site user, I want to be able to browse and search for recipes 
    1. Upon entering the site, users are automatically greeted with the page title and sub heading
    1. There is a clear call to action to sign up to browse the recipes
* As a new site user, I want to be able to understand the intent of the page
    1. Upon entering the page, it is clear the site is designed around food and cooking. 
* As a new site user, I want I want to understand easily how to navigate the page and access the facilities provided
    1. The navigation bar has clear and easy to understand links. These links are also dynamic to whether the user is signed in or not so they are only seeing the relevant options
### **Returning user testing**
* As a returning site user, I want to be able to log in
    1. Upon entering the site, there is the option in the nav bar to register and log in
* As a returning site user, I want to be able to view my recipes
    1. the user's profile page provides all of the recipes the user has submitted
* As a returning site user, I want to be able to edit and delete my recipes
    1. The recipes the user has submitted all show buttons to edit and delete the recipes. This is not visible to other users
* As a returning site user, I want to be able to add new recipes
    1. The form to enter a new recipe allows the user to instantly add a recipe to the site in the required format
### **Site owner testing:**
* As a site owner, I want recipes added via the site to be stored in the correct format in the database
    1. The form to add or edit a recipe validates the content to ensure all fields are complete and are in the correct format
* As a site owner, I want to be able to see who has added each recipe
    1. When a recipe is submitted, the user's _Id is stored in the database. This shows on the site as the user's username on each recipe

### **Performance testing:**
1. Tested website responsiveness using http://www.responsinator.com/
    1. Results: The website is responsive to all device sizes without any unnecessary x-scroll. 
1. All HTML pages were tested using https://validator.w3.org/
    1. Only 2 errors were found where buttons were used inside of an anchor tag.
1. Tested the CSS using https://jigsaw.w3.org/css-validator/
    1. No errors were found
1. Tested the website on the Google Chrome
    1. Results: The website was responsive and the elements performed in the way they were intended to
1. Tested the website on the Microsoft Edge browser
    1. Results: The website was responsive and the elements performed in the way they were intended to
1. Tested the website on the Firefox browser
    1. Results: The website was responsive and the elements performed in the way they were intended to
1. Tested the form validation worked correctly on each of the above browsers
    1. Results: The form correctly sent when the fields were completed as they should have been and did not when the fields had not been completed

# <a name="deployment"></a> Deployment
## <a name="github"></a> Github Pages
1. Create a new repository or access an existing repository
1. Click the green Gitpod button to launch the project in Gitpod
1. Create an index.html file
1. Add the file to the staging area using the git add Functional
1. Commit the file using the git commit function, adding an appropriate commentary
1. Push the file to GitHub using the git commit and git push functions
1. Refresh your GitHub repository and click the 'Settings' tab
1. Scroll to the GitHub Pages section and select a publishing source
1. Click 'Save'
1. Click the URL created within the Settings - GitHub Pages section

**To clone the repository for local deployment:** 
1. On the main page of the repository, click the down arrow Code button
1. Click the download icon under the relevant section to clone with either HTTPS, SSH or GitHub CLI 
1. In Git Bash, change the current directory to the location you want the directory to be stored
1. Type git clone and then paste the URL you copied in step 2
    1. An example for HTTPS: `git clone https://github.com/AaronHughes424/ShareYourRecipe`
1. Press enter - that's it, your clone has been completed! 

**To fork the repository:**
1. Navigate to the main page of the repository you wish to fork
1. Click the Fork button on the top right hand side of the page
## <a name="heroku"></a> Heroku
### How to deploy to Heroku

To deploy the app to Heroku from its [GitHub repository](https://github.com/AaronHughes424/ShareYourRecipe), the following steps were taken:

1. From the GitPod terminal, create **requirements.txt** and **Procfile** using these commands:

```console
pip3 freeze --local > requirements.txt
echo web: python app.py > Procfile
```

2. **Push** these files to GitHub
3. **Log In** to [Heroku](https://id.heroku.com/login)
4. Select **Create new app** from the dropdown in the Heroku dashboard
5. Choose a unique name ('recipe-nation') for the app and the location nearest to you
6. Go to the **Deploy** tab and under **Deployment method** choose GitHub
7. In **Connect to GitHub** enter your GitHub repository details and once found, click **Connect**
8. Go to the **Settings** tab and under **Config Vars** choose **Reveal Config Vars**
9. Enter the following keys and values, which must match those in the env.py file created earlier:

|**Key**|**Value**|
|:-----|:-----|
|IP|`0.0.0.0`|
|PORT|`5000`|
|SECRET_KEY|`<app secret key>`|
|MONGO_URI|`mongodb+srv://aaronhughes424:Jackson22@recipeshare.ul2rr.mongodb.net/recipe_share?retryWrites=true&w=majority`
|MONGO_DBNAME|`recipe_share`|

10. Go back to the **Deploy** tab and under **Automatic deploys** choose **Enable Automatic Deploys**
11. Under **Manual deploy**, select **master** and click **Deploy Branch**
12. Once the app has finished building, click **Open app** from the header row of the dashboard

# <a name="credits"></a> Credits
## <a name="content"></a> Content
All of the recipes and images added under the username 'aaronhughes' were sourced from https://www.bbcgoodfood.com
https://www.bbcgoodfood.com/recipes/shortbread-biscuits
https://www.bbcgoodfood.com/recipes/yummy-golden-syrup-flapjacks
https://www.bbcgoodfood.com/recipes/chocolate-fudge-cake
https://www.bbcgoodfood.com/recipes/new-york-cheesecake
https://www.bbcgoodfood.com/user/187365/recipe/creamy-garlic-mushrooms
https://www.bbcgoodfood.com/recipes/beef-stroganoff

The Code Institute:

Providing an indepth walkthrough of User Validation via materialize.css

Hero Image taken from:

https://unsplash.com/s/photos/cooking

## <a name="acks"></a> Acknowledgements

* My mentor Antonio Rodriguez who has provided me with guidance and support through the project

* My friends and family who helped to test the site and to add recipes

* Code institue slack who provided a fix for the updated mongoDB methods.
    