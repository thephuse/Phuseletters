Phuseletters
=================
Getting Started
----------------
Clone repo and create a duplicate of `responsive-template/newsletter.html` in the respective folder for the month and year.

When developing locally, create an `/images` directory within the folder for the month, and reference images using local paths, MailChimp will upload the files and change the references for you. 

When you have finished developing your newsletter locally, zip the folder containing both your html file and image files. 

MailChimp
-----------
To create the newsletter within MailChimp, select "Create Campaign (Regular Ol' Campaign)", select the "Phuseletters" list, and fill out Campaign info **more info needed**. Once you reach the "design" step, select the "Import -> Import from ZIP file" option. Upload your .zip file. This will upload all images referenced in the HTML to MailChimp's CDN, and change the references to them in your code. **If you have background images referenced in CSS, you will have to change these paths manually (background images should always be referenced both using CSS and using the `background` property of table or table cell)**

Ensure that you have selected the "Automatic CSS Inliner" option beneath the code editor, and send some test emails using the "Preview and Test" option. 

HTML Email Gotchas and Reminders
---------------------------------
(Not an exhaustive list). [Campaign Monitor is a great reference](http://www.campaignmonitor.com/resources/will-it-work/guidelines/)

- use images selectively: do not use them for important text information. If the designer has used non websafe fonts for headers or text, discuss what the best websafe alternative would be. We don't want important information to be hidden when images are disabled.
- Use alt text where appropriate (ex. logos), and ensure you specify the height and width of images within the html.
- Prefer specifying widths on table cells over tables
- background images should be referenced both in html using `background="url.jpg"` within a `table` or `td` tag, as well as in the CSS for the element. 
- Try to test in your desktop client, Gmail in the browser, and on your mobile device as a minimum. 

This Repo
-----------
Please do not make changes to the template file itself on the main branch without discussion. 
