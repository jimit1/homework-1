# What about box-sizing? What does * do??? Come back to this to solve this.

# Fix aside margin from top

# Things Changed

- Uploaded all images to S3 Bucket. I found that the file size of each images is pretty huge and so uploaded the images to s3 bucket and linked those images onto the html

- Added 
```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- Background image was attached to the css file which is a bad practice. Removed the image from css file, uploaded to s3 bucket, and then linked to the html

- Rather than giving div a class and then targetting the image inside seemed unnecessary. So removed the class from div and put it in image. Now my css is directly targetting the image now div. 

- changed the header class on div and renamed it to nav. Correspondingly changed the css to target nav and not header.

- the h1 was being targetted by nesting inside the header/nav class. But h1 can be directly targetted so removed the unnecessary class.

- Changed div class footer to directly footer to taget it. changed it correspondingly in css

- Header class should not be used in footer. so chanhged h2 to footer-top class and made same changes in css

- ("social-media-marketing", "online-reputation-management", "search-engine-optimization") had mix of just class or both id & class. Changed everything to id since I wanted to land on that section of the webpage when clicked on the nav bar. Correspondingly changed from . to # to target id not class

- since the color belonged to h1, changed to css location of color from nav to h1

- Removed float from nav div and added flexbox to nav with align center and justify-content:space-between. Also removed a lot of unnecessary code associated with floats since now flexbox is in use. so h1 and ul inside the nav doesn't need centring etc.

- Removed the unnecessary div inside nav before ul. Directly targetting the ul

- combined 2 different navs into 1. removed a lot of duplication inside.

- Removed an unnecessary div before the background image of class hero. wow this webpage developer was really bad!! Glad you hired me to refactor your code. Hi-5 to anyone who is reading this boring ass text block.

- Changed div class content to section + in css

- Changed div class benefits to aside + in css

- Since all h2 were being targetted the same way removed (#search-engine-optimization , #online-reputation-management , #social-media-marketing ) from the code and reduced 12 lines to 4.

- Ok did lots here. moved the "#search-engine-optimization, #online-reputation-management, #social-media-marketing" above. combined them since they are using the same lines of code, added flexbox. deleted float right and left. added div to separate out image and text sections, added some padding to separate them out. wow! so much!!

- Added a main section to nest the section and aside section of code. this way I could add flexbox and remove the float right that was on aside. works perfectly!

- Combined all h3 and simply called it h3 to target them all together. Reduced atleast 8-10 lines from code.

- why use three separate (.benefit-lead, .benefit-brand, .benefit-cost) when you can simply share the class and reduce so many lines from code. why would you ever have 3 separate classes! why! why would you ever do that!! now it is simply called benefit and I at the minimum reduced the code lenght in css by 20 odd lines. Wow! it is so clean now!

- now that we have a main section - adding the font to main rather than individually on section and aside. same with color

- fuck the margin at the bottom of the third tile (#social-media-marketing) was bothering the crap out of me. so separated it and removed the margin-bottom

- Or event better. only separate out the other top where margings are required. trying to reduce repetition and lenght of code.

- Targetting the image directly by adding the class on image rather than from div outside. 