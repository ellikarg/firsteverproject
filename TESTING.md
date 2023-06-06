# Alessio Mida -  Testing

![finished_site](https://github.com/ellikarg/firsteverproject/assets/132999023/ff1544d5-2710-4520-89ff-560afb546bc7)

Visit the deployed site: https://ellikarg.github.io/firsteverproject/index.html

- - -

## CONTENTS

* [AUTOMATED TESTING](#automated-testing)
  * [W3C Validator](#w3c-validator)
  * [Lighthouse](#lighthouse)
  * [WAVE Testing](#wave-testing)
* [MANUAL TESTING](#manual-testing)
  * [Testing User Stories](#testing-user-stories)
  * [Full Testing](#full-testing)
* [BUGS](#bugs)
  * [Solved Bugs](#solved-bugs)
  * [Known Bugs](#known-bugs)

During development I made use of Google Chrome Developer Tools to ensure everything was working correctly and to assist with troubleshooting when things were not working as expected. The automated and manual testing was unfortunately only done at the end.

I have gone through each page using Google Chrome Developer Tools to ensure that each page is responsive on a variety of different screen sizes and devices.

- - -

## AUTOMATED TESTING

### W3C Validator

[W3C](https://validator.w3.org/) was used to validate the HTML on all pages of the website. It was also used to validate the CSS. I have checked the HTML via direct input.

First, the validation stated errors with the aria-labels, but when I checked on the LMS and put them inside the ankor-element instead of the icon, it turned out without errors or warnings.

Checking the index page:<br><br>
![Validator_w3_index_page](https://github.com/ellikarg/firsteverproject/assets/132999023/416e8c48-1782-4264-887a-71c82da5672f)

Checking the photography page:<br><br>
![Validator_w3_photography_page](https://github.com/ellikarg/firsteverproject/assets/132999023/9010ee22-0fdf-42a7-b4f1-172a72102d05)

Checking the storytelling page:<br><br>
![Validator_w3_storytelling_page](https://github.com/ellikarg/firsteverproject/assets/132999023/f7aace52-ab19-424c-a223-cdea687dac76)


- - -

### Lighthouse
#### Mobile Results
I used Lighthouse within the Chrome Developer Tools to test the performance, accessibility, best practices and SEO of the website. 

The scores for the mobile view were:
<ul>
  <li>for the index page: between 96 and 100</li>
  <li>for the photography page: between 96 and 100 with the exception of performance (with only 66) since the pictures were in jpg and not optimized. After optimization and convertion to webp the scores were: between 99 and 100</li>
  <li>for the storytelling page: between 81 and 100 with the performance being only at 78 (the rest at 98 and 100). This is as well due to the images although I already optimized them and the cache</li>
 </ul>
 
#### Desktop Results

The scores for the desktop vew were:
<ul>
  <li>for the index page: 100 for all pages</li>
  <li>for the photography page: between 90 and 100 </li>
  <li>for the storytelling page: between 98 and 100 with accessibility being 98 because on of the wrong sequentially-descending order of the headings on this page (it went from h1 directly to h3). I'm glad this was noticed in this testing! After the fixing of the order the scores were between 98 and 100</li>
 </ul>

- - -

### WAVE Testing

[WAVE](http://wave.webaim.org/) (Web Accessibility Evaluation Tool) allows developers to create content that is more accessible to users with disabilities. It does this by identifying accessibility and WGAC errors.

I have used the WAVE testing tool to try and ensure there are no accessibility issues with my site. There were no errors shown for the the pages.

- - -

## MANUAL TESTING

### Testing User Stories

| Goals | How are they achieved? | Image |
| :--- | :--- | :--- |
| `First Time Visitors` |
|  |  |  |
| Get to know Alessio Mida as a creative photographer | The front page displays a small paragraph about him as well as a quotation that he really likes. | :--- |
| Get an impression of his latest work in photography | The photo gallery on the photography-page shows some of his photographs devided in three categories. | :--- |
| Be able to read his latest travel stories | The storytelling page displays three stories of his latest travel to Palestine, Israel and Jordan. | :--- |
|`Returning Visitors`|
|  |  |  |
| Get updates about new stories | The storytelling page will be updated regularly and a link from the shorter instagram posts will redirect the readers to the webpage in order to be able to read the whole story. | :--- |
| Get/remember his instagram and facebook contact | Visitors can follow the links on the bottom of each page to get directly to his facebook and instagram pages. | :--- |
| Show others his work | Returning visitors can use the site to show his work to others who might be interested in contacting him for a photography session. | :--- |

- - -

### Full Testing

Full testing was performed on the following devices:

* Laptop:
  * Dell Latitude E7240
* Mobile Devices:
  * Huawei P30 light
  * iPhone SE
  * 

Each device tested the site using the following browsers:

* Google Chrome
* Safari
* Firefox

Additional testing was taken by friends and family on a variety of devices and screen sizes. A Big thank you to all of them!

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| `Navbar` |
|  |  |  |  |  |
| Bookworm Logo & Title | When clicked the user will be redirected to the home page. | Clicked Logo and title | Redirected to the home page. | Pass |
| Home Page Link | When clicked the user will be redirected to the home page.| Clicked link | Redirected to the home page. | Pass |
| Search Link | When clicked the user will be redirected to the search page. | Clicked link | Redirected to the search page. | Pass |
| Bookshelves Link (Logged in users only) | When clicked the user will be redirected to the bookshelves page. | Clicked link | Redirected to the bookshelves page | Pass |
| Books Link (Logged in users only) | When clicked the user will be redirected to the books page. | Clicked link | Redirected to the books page | Pass |
| Profile Link (Logged in users only) | When clicked the user will be redirected to the profile page. | Clicked link | Redirected to the profile page | Pass |
| Log in Link (Only shown if user not in session) | When clicked the user will be redirected to the log in page. | Clicked link | Redirected to the log in page | Pass |
| Register Link (Only shown if user not in session) | When clicked the user will be redirected to the register page. | Clicked link | Redirected to the register page  | Pass |
| Log out Link (Logged in users only) | When clicked the user will be redirected to the home page and a flash message displayed to let the user know they have been logged out successfully. | Clicked link |Redirected to the home page and a flash message displayed to let me know I have been logged out | Pass |
| `Footer` |
|  |  |  |  |  |
| Bookworm Title | When clicked the user will be redirected to the home page. | Clicked Logo and title | Redirected to the home page. | Pass |
| Copyright year | The copyright should display the correct year - this is a javascript function that checks what the current year is and injects it into the footer | Checked the year | Displaying the correct year | Pass |
| `Home Page` |
|   |   |   |   |
| Register link in the blurb | When clicked the user will be redirected to the register page. | Clicked link  | Redirected to the register page | Pass |
| Search link in the blurb | When clicked the user will be redirected to the search page. | Clicked link | Redirected to search page | Pass |
| `Log in Page` |
| Username input - empty | This is a required field so the form should not submit if empty | Tried to submit the form with this field empty | Tooltip tells me this field is required | Pass |
| Password input empty | This is a required field so the form should not submit if empty | Tried to submit the form with this field empty | tooltip tells me this field is required |  Pass |
| log in button | Saves the user to session and redirects to the profile page. Flash message shown welcoming the user | Submitted form | Redirected to the profile page and flash message shown | Pass |
| Incorrect username or password used | A flash message should display saying username/password incorrect - this is defensive programming - not letting user know which input is incorrect | Incorrect username/password entered | Message flashes to let the user know they have entered an incorrect username/password | Pass |
| Link to register page |  This should redirect the user to the register page | Clicked link | Redirected to the register page | Pass |
| `Register Page` |
| | | | | | |
| Username input | The username should be 5 characters minimum | Entered username less than 5 characters long | tooltip lets the user know they have not entered enough characters | Pass |
| Username input - empty | The username is a required field, so should not submit with no value | Tried to submit form with no value entered | Tooltip lets user know this value is required | Pass |
| Username input | If username is in use, message should flash to user | entered an in use username | Message flashed to say username already in use | Pass|
| Email input | The email input should include an email address  | Entered plain text | Tooltip tells user to use an email address here | Pass |
| Email input - empty | The email is a required field, so should not submit with no value | Tried to submit form with no value entered | Tooltip lets user know this value is required | Pass |
| Password input | This field should be at least 5 characters long | Entered password less than 5 characters long | Tooltip tells user the password should be at least 5 characters long | Pass |
| Password input - empty | The password is a required field, so should not submit with no value | Tried to submit form with no value entered | Tooltip lets user know this value is required | Pass |
| Register button | Should redirect user to the log in page and a registration successful message flashed | Created new user and submitted form | Redirected to the log in page and message flashed | Pass |

 - - -

## BUGS

### Solved Bugs

| No | Bug | How I solved the issue |
| :--- | :--- | :--- |
| 1 | When I added the accordion to the book search results, the accordion would open and close on all books together when triggered due to the accordion being created in the for loop, the id was identical for all results. | To enable each accordion to open and close individually I needed to find a way to create a unique ID on every iteration of the for loop. Initially I considered taking the title and using the python method replace to remove any spaces in the title. However this would have been a problem if there were two books with identical names. I posed my question on slack and Daisy suggested using a loop.counter. On researching this I discovered it is only applicable to Django, however something very similar exists in Jinja - a loop.index. By using the loop.index in the id attribute I was able to create a unique ID for each book and this allowed the accordion to be opened and closed on each book individually.  |
| 2 | The bootstrap modal for deleting a bookshelf was displaying but was hidden under the backdrop, making it impossible to use the modal buttons or to exit out of the modal. ![Modal Bug](documentation/testing/modal-bug.png) | I initially tried moving the modal code within the file but this made no difference. Upon searching google for bootstrap modal greyed out I found the following [article](https://weblog.west-wind.com/posts/2016/Sep/14/Bootstrap-Modal-Dialog-showing-under-Modal-Background?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+RickStrahl+%28Rick+Strahl%27s+WebLog%29). I tried a few of the fixes, which didn't work before finding that the fix to remove the backdrop did work. This is not an ideal fix, but works for the moment until I can research this issue further and find a more elegant solution. |
| 3 | Users could try to view the bookshelves page by entering the URL for the bookshelves page whilst not logged in and would be presented with a keyerror page. This was not a great user experience as it did not display any information that would be useful to a user as to what the issue was. | Upon checking my routes for the bookshelves page, I found that I had not included any defensive programming to prevent a user from trying to view the bookshelves page without being logged in. I have Added the logic to check whether a user is in session, and if not to present a flash message. This provides the user with a better overall experience on the site and provides them with some useful feedback - letting the user know they need to be logged in to view their bookshelves and then redirecting them to the log in page. |
| 4 | Users could try to view the books page by entering the URL for the books page whilst not logged in and would be presented with a keyerror page. This was not a great user experience as it did not display any information that would be useful to the user as to what the issue was. | Upon checking my view_books route, I found that I had not included any defensive programming that would prevent a user from accessing the page without being logged in. I have added the logic to check whether the user is in session, and if not to present a flash message. This provides the user with a better overall experience on the site and provides them with some useful feedback - letting the user know they need to be logged in to view the books page and redirecting them to the log in page. |
| 5 | No user feedback when user enters a bookshelf name already in use | I had originally created this columns in the database to be a unique field. As I thought that a user wouldn't want to have two bookshelves with the same name. This then raised the issue that the bookshelf name could only be used once by anyone - so two users couldn't create a to be read shelf. This was not a great user experience, and I could either change it so that the column wouldn't be unique, or I could just handle the error by flashing an error message to the user telling them this bookshelf name was already taken. I decided that it would be a better user experience to allow all users to be able to make a shelf with the same name. I made the changes to my models.py and migrated these changes using flask migrate. I then pushed these changes to GitHub and ran the migrations in the heroku console. Unfortunately, the migrations were not being deployed to the live site, despite them working on the local version of the site. I performed a lot of research on slack and google, spoke to peers about the problem, referred back to the lesson material and eventually contacted tutor support regarding the issue. Tutor support recommended that if I had pushed my changes to GitHub and they were still not being picked up by Heroku after running the migration, it was most likely that they was some issue with my data in the database and I would have to reset my postgres database, and run migrations again. As I had tried all other suggestions without any success, I have had to reset the databases for users and bookshelves in order to make the migrations to the live site. I have tested this on the live site and users can now create the same bookshelf more than once, which means that several users can use the same name for their bookshelves. |
| 6 | The star ratings seem to be misaligned since the app has been deployed. ![Stars alignment](documentation/testing/stars-alignment.png)| I went back and looked at the original code snippet used to create this effect and noticed that they were using the star whereas I was using a bootstrap icon on the page for the blank star, but not for the css fill. By changing the blank star shown on the page to the star rather than a bootstrap icon I was able to solve the issue of the hover effect not lining up correctly. |
| 7 | If a user tries to save a book with no authors listed in the google books API, an error occurs when they try to save that book to a bookshelf. ![No author error](documentation/testing/no-author-error.png) | I decided the best way to deal with this problem would be to use a ternary condition for the author in the dictionary created of the books information to be pre-populated to the form. If there was no author listed on the book, a blank string would be used, else the authors details from the API call would be used. |
| 8 | Despite having my debug=False in my heroku vars, I was still having error tracing show on the deployed site. | [Suzy](https://github.com/suzybee1987) let me know that this is due to the fact that heroku vars are read as a string, so therefore it is actually reading it as true. This issue has been solved by removing this variable from my config vars in heroku. |

- - -

### Known Bugs

| No | Bug | |
| :--- | :--- | :--- |
| 1 | When performing searches using the google books API, sometimes it is not returning a result, which results in a flash message being shown. I have noted that during development the API was returning results for certain terms, but when deployed these search terms would not return a result. I plan to look further into this issue as to why it is not returning a result and see if there is a way to filter out book results that are missing attributes. | |
| 2 | Some books when shelved are pulling in a different book than the one selected. I have taken the unique volume ID and performed a check on the google books page and the ID is correct for the book selected, so there would appear to be an issue with the request to the API. This is something that I will need to look into further to discover why it is returning the wrong information. | ![Wrong book being populated](documentation/testing/wrong-book-populated.gif) |
| 3 | During development I used many search terms to test the search function of the site. However I have found that on deployment some of the search terms that returned a result in development are not returning a result and so are showing the flash message to the user. This is something that I will need to look into further as I know that the search returns a result. I feel that perhaps it may be because some books may be missing parameters. | |
| 4 | The buttons on the accordion are not aligned to the bottom of the footer. I would like to adjust this so that the buttons on all book results line up at the bottom of the footer. | ![Buttons not aligned](documentation/testing/buttons-align.png) |
| 5 | When opening an accordion on a book, the other books on the same row also expand showing whitespace. I would like to change this so that only the book being opened expands. | ![Accordion issue](documentation/testing/accordion-issue.gif) |
| 6 | I tried to add defensive programming to the profile page to prevent anyone from being able to view that page unless signed in by using similar defensive programming used throughout the project (if 'user' not in session). This worked fine in local development, however once I deployed to the live site, I couln't complete log in and access the profile page as I would hit a 500 error instead. I have reverted the code by removing the defensive programming from the profile route for now, so that users may log in and use the site, however I am aware of the issue and that this will need some additional work to get the defensive programming working. For the moment there is nothing sensitive on the profile page, and I have tested and checked that despite this page being available to a user who is not signed in, they are not able to access anything else on the site specific to a user. |
