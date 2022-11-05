# Mission_to_Mars

What You're Creating
This new assignment consists of three technical analyses. You will submit the following deliverables:

Deliverable 1: Scrape Full-Resolution Mars Hemisphere Images and Titles
Deliverable 2: Update the Web App with Mars Hemisphere Images and Titles
Deliverable 3: Add Bootstrap 3 Components
Files
Use the following links to download the Challenge starter codes.

Download the starter code.Links to an external site.

Download the updated index.html file.Links to an external site.

Deliverable 1: Scrape Full-Resolution Mars Hemisphere Images and Titles (40 points)
Deliverable 1 Instructions
Using BeautifulSoup and Splinter, you’ll scrape full-resolution images of Mars’s hemispheres and the titles of those images.

REWIND
For this deliverable, you’ve already done the following in this module:

Lesson 10.3.2: Use Splinter and Beautiful Soup
Lesson 10.3.4: Scrape images
Lesson 10.5.1: Use Flask to create a web app
Lesson 10.5.2: Update the code for the web app
Lesson 10.5.3: Connect MongoDB with the web app
Follow the instructions below to complete Deliverable 1.

Make a copy of your Mission_to_Mars.ipynb file, and rename it Mission_to_Mars_Challenge.ipynb.
Download the Mission_to_Mars_Challenge_starter_code.ipynb, copy the starter code, and paste at the end of your Mission_to_Mars_Challenge.ipynb file.
In Step 1, use your browser to visit the Mars HemispheresLinks to an external site. website to view the hemisphere images.
The Mars hemisphere webpage

Use the DevTools to inspect the page for the proper elements to scrape. You will need to retrieve the full-resolution image for each of Mars's hemispheres.
NOTE
There is more than one way to get the images and titles.

In Step 2, create a list to hold the .jpg image URL string and title for each hemisphere image.
In Step 3, write code to retrieve the full-resolution image URL and title for each hemisphere image. The full-resolution image will have the .jpg extension.
Loop through the full-resolution image URL, click the link, find the Sample image anchor tag, and get the href.
HINT
If you’d like a hint on how to get started, that’s totally okay. If not, that’s great too. You can always revisit this later if you change your mind.

Follow the steps below to use one common approach:

Find the HTML tag that holds all the links to the full-resolution images, or find a common CSS element for the full-resolution image.
Using a for loop, iterate through the tags or CSS element.
Create an empty dictionary, hemispheres = {}, inside the for loop.
Use the for loop to complete the following actions: a) click on each hemisphere link, b) navigate to the full-resolution image page, c) retrieve the full-resolution image URL string and title for the hemisphere image, and d) use browser.back() to navigate back to the beginning to get the next hemisphere image.
Save the full-resolution image URL string as the value for the img_url key that will be stored in the dictionary you created from the Hint.
Save the hemisphere image title as the value for the title key that will be stored in the dictionary you created from the Hint.
Before getting the next image URL and title, add the dictionary with the image URL string and the hemisphere image title to the list you created in Step 2.
In Step 4, print the list of dictionary items. Your list should look like the following image:
The dictionary that holds the image URL strings and the hemisphere titles for each hemisphere.

After you have confirmed that you have the image URLs and titles for all four hemisphere images, quit the browser by executing Step 5.
Deliverable 1 Requirements
You will earn a perfect score for Deliverable 1 by completing all requirements below:

Code is written that retrieves the full-resolution image and title for each hemisphere image (10 pt)
The full-resolution images of the hemispheres are added to the dictionary. (10 pt)
The titles for the hemisphere images are added to the dictionary. (10 pt)
The list contains the dictionary of the full-resolution image URL string and title for each hemisphere image. (10 pt)
Deliverable 2: Update the Web App with Mars’s Hemisphere Images and Titles (40 points)
Deliverable 2 Instructions
Using your Python and HTML skills, you’ll add the code you created in Deliverable 1 to your scraping.py file, update your Mongo database, and modify your index.html file so the webpage contains all the information you collected in this module as well as the full-resolution image and title for each hemisphere image.

REWIND
For this deliverable, you’ve already done the following in this module:

Lesson 10.3.6: Export your script as a Python file
Lesson 10.5.1 Use Flask to create a web app
Lesson 10.5.2: Update the code for the web app
Lesson 10.5.3: Connect MongoDB with the web app
Follow the instructions below to complete Deliverable 2.

Export the Mission_to_Mars_Challenge.ipynb file as a Python file, and save it as Mission_to_Mars_Challenge.py.
In the def scrape_all() function in your scraping.py file, create a new dictionary in the data dictionary to hold a list of dictionaries with the URL string and title of each hemisphere image.
Below the def mars_facts() function in the scraping.pyfile, create a function that will scrape the hemisphere data by using your code from the Mission_to_Mars_Challenge.py file. At the end of the function, return the scraped data as a list of dictionaries with the URL string and title of each hemisphere image.
Run the app.py file, then check your Mongo database to make sure that you are retrieving all of the data.
Modify the index.html file to access your database, and retrieve the img_url and title as you loop through the dictionary in the database using {% for hemisphere in mars.hemispheres %}. The dictionary in the mars hemispheres database is the dictionary that was created from the Hint after Step 3 in Deliverable 1.
If you’d like a hint on coding the syntax for rendering Mongo database objects in your index.html file, that’s totally okay. If not, that’s great too. You can always revisit this later if you change your mind.

HINT
Run the app.py file, open the index.html file, and click the "Scrape New Data" button.
After you have scraped the data, confirm that your webpage has the full-resolution images and the titles of the four hemisphere images, like the image below.
The full-resolution images and titles of the four hemispheres of Mars.

Save your Mission_to_Mars_Challenge.ipynb file, the updated scraping.py file, and the updated index.html file.
Deliverable 2 Requirements
You will earn a perfect score for Deliverable 2 by completing all requirements below:

The scraping.py file contains code that retrieves the full-resolution image URL and title for each hemisphere image (10 pt)
The Mongo database is updated to contain the full-resolution image URL and title for each hemisphere image (10 pt)
The index.html file contains code that will display the full-resolution image URL and title for each hemisphere image (10 pt)
After the scraping has been completed, the web app contains all the information from this module and the full-resolution images and titles for the four hemisphere images (10 pt)
Deliverable 3: Add Bootstrap 3 Components (20 points)
Deliverable 3 Instructions
For this part of the Challenge, update your web app to make it mobile-responsive, and add two additional Bootstrap 3 components to make it stand out.

REWIND
For this deliverable, you’ve already done the following in this module:

Lesson 10.6.1: Customize the appearance of a webpage
As you update your app, keep the following questions in mind:

Is this page clean?
Does the page stand out from other pages?
Follow the instructions below to complete Deliverable 3.

Use the Bootstrap 3 grid systemLinks to an external site. examples to update your index.html file so your website is mobile-responsive. Use the DevTools to test the responsiveness of your website.
Click on the Toggle Device Toolbar icon to open the UI that enables you to simulate responsiveness.
Choose a device to test your webpage, as shown in the following image:
Using the Toggle Device Toolbar for mobile responsive devices.

Add two other Bootstrap 3 components from this listLinks to an external site.. Examples include:
Styling the "Scrape New Data" button.
Customizing the facts table.
Adding the hemisphere images as thumbnails, like the image below.
The full-resolution images as thumbnails, and titles of the four Mars hemisphere images.

Deliverable 3 Requirements
You will earn a perfect score for Deliverable 3 by completing all requirements below:

The webpage is mobile-responsive (10 pt)
Two additional Bootstrap 3 components are used to style the webpage (10 pt)
Submission
Once you’re ready to submit, make sure to check your work against the rubric to ensure you are meeting the requirements for this Challenge one final time. It’s easy to overlook items when you’re in the zone!

As a reminder, the deliverables for this Challenge are as follows:

Deliverable 1: Scrape High-Resolution Mars Hemisphere Images and Titles
Deliverable 2: Update the Web App with Mars Hemisphere Images and Titles
Deliverable 3: Add Bootstrap 3 Components
Upload the following to your Mission-to-Mars GitHub repository:

The Mission_to_Mars_Challenge.ipynb file with all the code used for scraping.
An updated scraping.py file.
The app.py file.
The index.html file in the template folder and any CSS stylesheets.
A README.md that describes the purpose of the repository. Although there is no graded written analysis for this challenge, it is encouraged and good practice to add a brief description of your project.
To submit your challenge assignment for grading in Bootcamp Spot, click Start Assignment, click the Website URL tab, then provide the URL of your Mission-to-Mars GitHub repository, and then click Submit. Comments are disabled for graded submissions in BootCampSpot. If you have questions about your feedback, please notify your instructional staff or the Student Success Manager. If you would like to resubmit your work for an improved grade, you can use the Re-Submit Assignment button to upload new links. You may resubmit up to 3 times for a total of 4 submissions.
