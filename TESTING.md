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

I also used [W3C CSS Validation](https://jigsaw.w3.org/css-validator/validator) to validate my css file, which also resulted in no errors.

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
  * iPhone 8

Each device tested the site using the following browsers:

* Google Chrome
* Safari
* Firefox

Additional testing was taken by friends and family on a variety of devices and screen sizes. A Big thank you to all of them!
<br><br>

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
| `Navbar` |
| Page's Logo (camera icon) | When clicked the user will be redirected to the home page. | Clicked Logo | Redirected to the home page. | Pass |
| Link "Home" | When clicked the user will be redirected to the home page.| Clicked link | Redirected to the home page. | Pass |
| Link "Photography" | When clicked the user will be redirected to the page about his photography. | Clicked link | Redirected to the photography page. | Pass |
| Link "Storytelling" | When clicked the user will be redirected to the page about his storytelling. | Clicked link | Redirected to the storytelling page | Pass |
|  |  |  |  |  |
| `Footer` |
| Facebook Link (icon) | When clicked the user will be redirected to the photographer's facebook account. | Clicked Icon | Redirected to the facebook account | Pass |
| Instagram Link (icon) | When clicked the user will be redirected to the photographer's instagram account. | Clicked Icon | Redirected to the instagram account | Pass |

 - - -

## BUGS

### Solved Bugs

| No | Bug | How I solved the issue |
| :--- | :--- | :--- |
| 1 | One bug that I spent a lot of time fixing on was that the gallery pictures would overlap the h3-headings when displayed in the grid with only one column (for small screens) | In the end I managed to fix it with a really good hint from my mentor: using the dev tools to make a border around each div-container of the grid-structure and then consequently checking all margin- and padding- and gap-values for the different screen sizes and how they behave when changed from one to another. |
| 2 | Another bug that took me a bit to solve was the round image-container on the index page, because it would always loose its shape when viewed on different screen sizes although I had given it a fixed size | In the end I watched many flex-box tutorials and when my mentor showed me the help with the borders around the flexbox-items, I understood that I have to use another div-element as flex-element in order for the round image-container not to be responsive, but the div around it. |


- - -

### Known Bugs

| No | Bug | |
| :--- | :--- | :--- |
| 1 | Two of the gallery images were oversized on the iPhone 8 in the safari browser | Strangely, on an iPhone SE (also in the safari browser), this was not a problem at all. |
