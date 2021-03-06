# [Where to Next](https://hollyford.github.io/where-to-next/)

# A travel blog by Holly

## Contents
1. Summary
1. UX
    1. Strategy
    1. Scope
    1. Structure
    1. Skeleton
    1. Surface
1. Features
    1. Existing features
    1. Featured left to implement
1. Bugs
1. Technologies used
1. Testing
1. Deployment
1. Credits
    1. Content
    1. Media
    1. Acknowledgements
# Summary
This is a travel blog website which provides a short overview of the site owner's top 10 destinations in Europe. 

The site includes a Google Map with markers showing recommended places to visit, eat and stay. 

There is also a feedback section where site users can make recommendations for destinations for the site owner to visit next. They can also recommend places to visit, stay and eat in the destinations already on the site. In addition, the form the site user submits will ask for permission for the site owner to contact them for further information and whether they can be credited in the recommendation when it is published on the website.
# UX
## Strategy
### **Site user's Goals:**
The users are people who love to travel, want to learn about popular destinations, want to plan their next trip or simply want to read about the site owner's travels
*  As a new site user, I want to be able to understand the intent of the page
* As a new site user, I want to understand easily how to navigate the page and access the facilities provided
* As a returning site user, I want to be able to easily reach a section of the site previously viewed without many steps to get there
* As a site user, I want to view the top 10 travel destinations in Europe
*  As a site user, I want to have links to the recommended restaurants, places to stay and activities where appropriate
*  As a site user, I want to be able to provide feedback on the site
*  As a site user, I want to be able to provide my own recommendations 

### **Site owner's goals:**
*  As a site owner, I want to be able to receive value feedback on the site, including recommendations from the site users

## Scope
**Functional requirements:**
- Google Maps API
- EmailJS API
- Navigation bar which is simple and easy to navigate
- Feedback form which uses validation to ensure value content is submitted

**Content requirements:**
- Images of destinations
- Description of each destination
- Google Map for each destination 
- Customer markers within the maps of recommended places to stay, eat and things to do
- clickable markers to provide a short piece of information about the recommendation and links to external sources where appropriate

## Structure
**Interaction design:**
- User friendly interface
- Responsive and visible links which change on hover
- Ability to exit pop ups

**Information Architecture:**
- Navigation bar at the top of the page - sticky to the top so always visible
- Responsive navigation bar - adjusting for mobile
- Images of the appropriate viewing size, minimising for mobile
- All features appropriate size for mobile and desktop viewing
- All information is appropriate and relative to the subject and not misleading or hard to find

## Skeleton

Please click the below link to view the wireframe mock up of the website in mobile, tablet and desktop sizing

[Where to next wireframe](assets/wireframes/w2n.pdf)

## Surface
The intention of the surface design of the website is intended to be 'whimsical'. 
* The font family chosen from Google Fonts is 'pompiere'
* The colour selections are light and airy with the following colours selected for the colour scheme: 
    * dark-lava: #4a4238ff;
    * shiny-shamrock: #66a182ff;
    * middle-red: #e2856eff;
    * lavender-web: #e5eafaff;
    * cg-blue: #007ea7ff;
* The colour scheme was selected using the colour scheme creator: [Coolors.co](https://coolors.co/)

# Features

### **Existing Features**

Feature | Details
----------|---------
Map | The site includes a map which is customised for each location using arrays of latitudes and longitudes for each destination 
Map Markers | For each destination, the map will also provide customised recommendation markers using an array of latitudes and longitudes along with personalised marker icons and content boxes
Destination buttons | Each button will trigger any current content on the page to be hidden and the content for the selected destination to become visible. In addition to the maps and markers detailed above, this will show an image of the destination along with text detail describing each destination
Contact form | The contact form enables the site user to submit feedback and recommendations whilst also providing consent to be contacted again and/or to be quoted on the site. The form also includes validation to ensure content is provided within the required fields of the form to ensure value content is sent
Home button | the home button resets the page back to its original state with the main page image and no destination information showing
Feedback button | The feedback button on the top right hand side of the page takes the user down to the bottom of the page where the feedback form is located


### **Features Left to implement and improvement ideas**
All of the features in the initial scope of the site have been implemented. However, some improvement ideas have been identified
 Feature | Details
----------|---------
Map Markers | The marker icons selected work well for the page but there are some additional icons which could have been used instead. For example, a church icon where a church has been recommended
Destination buttons | The destination buttons could be included within a sub section of the nav bar to be more visually appealing
Contact form | The validation on the contact form currently ensures that each of the required fields have a minimum of three characters. I would like to refine this further with specific validation for each box
Images | Link to smaller images or store these locally to improve the loading time of the page

# Bugs

Bug | fix
--|--
The submit button in the feedback form would not trigger an email | Added onsubmit="event.preventDefault(); to the form HTML to prevent the form from completing the 'submit' function which effectively refreshed the web Pages. This enabled the email event to be triggered
When a new destination was selected, this appeared underneath the existing destination content | A class was added to each div, image and the map to ensure their initial state was hidden. The addClass and removeClass functions were then used to add/remove these classes as appropriate to ensure the correct content was showing for the button the user selected

# Technologies Used

* Bootstrap - https://getbootstrap.com/
* JavaScript
* Emailjs
* Google Maps
* Google fonts - https://fonts.google.com/
* www.validator.w3.org
* http://www.css-validator.org/
* Git
* Gitpod
* GitHub
* Google Chrome
* http://www.responsinator.com/
* Chrome Dev Tools
* https://coolors.co/

# Testing

**New site user testing:**
1. As a new site user, I want to be able to understand the intent of the page
    1. Upon entering the site, users are automatically greeted with the page title and sub heading
    1. There is a clear call to action to select one of the destination buttons
1. As a new site user, I want to understand easily how to navigate the page and access the facilities provided
    1. The sub heading of the page clearly shows how to use the page in a short and meaningful sentence
    1. The destination buttons are responsive when hovered over

**Returning site user testing:**
1. As a returning site user, I want to be able to easily reach a section of the site previously viewed without many steps to get there
    1. The destination buttons are prominent on the page for the returning user to quickly return to where they were previously
1. As a site user, I want to view the top 10 travel destinations in Europe
    1. The top 10 travel destinations are detailed in the buttons which are prominent on the page
    1. This user experience can be improved by highlighting that these are the top 10 destinations
1. As a site user, I want to have links to the recommended restaurants, places to stay and activities where appropriate
    1. When the destination is selected, a custom map opens up with markers. Within these markers, there is a description of the recommendation. Where it is a food or accommodation recommendation, links are provided to external sources
    1. Signage on the page can be improved to direct the site user to click on the markers to obtain the content
1. As a site user, I want to be able to provide feedback on the site
    1. There is a form at the bottom of the page which is fixed so it is always visible
    1. There is a link on the header which, when clicked, navigates to the form for the user to complete
1. As a site user, I want to be able to provide my own recommendations 
    1. There is a form at the bottom of the page which is fixed so it is always visible
    1. There is a link on the header which, when clicked, navigates to the form for the user to complete

**Site owner testing:**

As a site owner, I want to ensure the site is visually appealing
1. As a site owner, I want to be able to receive value feedback on the site, including recommendations from the site users 
    1. There is a form at the bottom of the page which is fixed so it is always visible
    1. There is a link on the header which, when clicked, navigates to the form for the user to complete
    1.
     The form has validation to ensure that it cannot be submitted without content in the name, email address and feedback fields

**Performance testing:**

1. Tested website responsiveness using http://www.responsinator.com/
    1. Results: The website is responsive to all device sizes
1. Tested the image size to ensure no image is to large and impacting the website loading times. I used the Google Dev Tools - Network
    1. Results: The site loading time is sub optimal. The total website loading time is 1.54s which can be improved
    1. This has been added to the improvement table within the features section
1. Tested the HTML using https://www.freeformatter.com/html-validator.html I would normally use https://validator.w3.org/ but there is currently an error with the server and results are not available
    1. Results - index.html: Three errors were recorded
        1. Malformed byte sequence: “e9”. At line 109, column 59
        1. Malformed byte sequence: “f6”. At line 223, column 98
        1. Malformed byte sequence: “e8”. At line 449, column 66
    1. The errors are created by Accent Marks on characters within the text content 
1. Tested the CSS using http://www.css-validator.org/
    1. Results - style.css: The validator does not recognise #4a4238ff or #66a182ff as valid color 3 or 6 hexadecimals numbers
    1. The colours currently work correctly within the browsers however, this is something which will need further investigation
1. Tested the website on the Google Chrome browser Version 87.0.4280.88 (Official Build) (64-bit)
    1. Results: The website was responsive and the elements performed in the way they were intended to
1. Tested the website on the Microsoft Edge browser Version Version 87.0.664.66 (Official build) (64-bit)
    1. Results: The website was responsive and the elements performed in the way they were intended to
1. Tested the website on the Firefox browser Version 82.0.3 (64-bit)
    1. Results: The website was responsive and the elements performed in the way they were intended to
1. Tested the form validation worked correctly on each of the above browsers
    1. Results: The form correctly sent when the fields were completed as they should have been and did not when the fields had not been completed
2. Tested the email was sent correctly using the console log
    1. Results: The console log confirmed the function had run correctly with: SUCCESS r {status: 200, text: "OK"}. In addition to this, an email was successfully received with the content added to the form
# Deployment
**GitHub Pages**
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
    1. An example for HTTPS: `git clone https://github.com/hollyford/where-to-next.git`
1. Press enter - that's it, your clone has been completed! 

**To fork the repository:**
1. Navigate to the main page of the repository you wish to fork
1. Click the Fork button on the top right hand side of the page

# Credits
### Content

 No.  | URL  | Description
 --|--|--
 1 | [europeanbestdestinations](https://www.europeanbestdestinations.com/european-best-destinations-2020/) | The text content of the divs which appear when a destination button is selected was copies from this website. The content was copies for the following destinations: Colmar, Athens, Tbilisi, Vienna, Cascais, Sibu, Namur, Rijeka, Paris, Bydgoszcz. These were the top 10 European destinations at the time of the page being created
 2 | [Google](https://www.google.co.uk/maps?hl=en&tab=wl) | Used to collate the latitude and longitudes for each destination and the customer markers for each map iteration 
 3 | [appspot](http://kml4earth.appspot.com/icons.html) | Used to source custom icons for the markers added on each map iteration
 4 | [Booking.com](https://www.booking.com/hotel/fr/hostellerie-le-marechal.en-gb.html?aid=356980;label=gog235jc-1DCAsoTUIXaG9zdGVsbGVyaWUtbGUtbWFyZWNoYWxIM1gDaFCIAQGYAQm4ARfIAQzYAQPoAQGIAgGoAgO4AquB9P4FwAIB0gIkNGQ4ODFkMDMtMmEzZS00Y2ZhLWI2M2EtZDg3ZTFiMGQ2YTEy2AIE4AIB;sid=8f5d6c7740e4b688a551571a0ae3738e;dist=0&keep_landing=1&sb_price_type=total&type=total&) | Used for the marker and the text content for a place to stay in Colmar. 
 5 | [The Crazy Tourist](https://www.thecrazytourist.com/15-best-things-colmar-france/) | Used to add content for the marker for Maison Pfister in Colmar
 6 | [lasoicolmar](https://www.lasoicolmar.fr) & Google.co.uk | Used to add the text content for the marker for a place to eat in Colmar
 7 | https://www.timeout.com/athens/restaurants/best-restaurants-in-athens & https://klimataria.gr/ | Used for the text content of the marker for a place to eat in Athens
 8 | [Booking.com](https://www.booking.com/searchresults.en-gb.html?aid=356980&label=gog235jc-1DCAIoXDgbSAlYA2hQiAEBmAEJuAEXyAEM2AED6AEB-AECiAIBqAIDuAKVm_n-BcACAdICJDM3OTQ4NTcxLWIxN2UtNDhmNi1iZjQwLTJmNjdkMDFlNGMyNdgCBOACAQ&sb=1&sb_lp=1&src=country&src_elem=sb&error_url=https%3A%2F%2Fwww.booking.com%2Fcountry%2Fgr.en-gb.html%3Faid%3D356980%3Blabel%3Dgog235jc-1DCAIoXDgbSAlYA2hQiAEBmAEJuAEXyAEM2AED6AEB-AECiAIBqAIDuAKVm_n-BcACAdICJDM3OTQ4NTcxLWIxN2UtNDhmNi1iZjQwLTJmNjdkMDFlNGMyNdgCBOACAQ%3B&ss=Athens%2C+Attica%2C+Greece&is_ski_area=0&ssne=Greece&ssne_untouched=Greece&checkin_year=&checkin_month=&checkout_year=&checkout_month=&group_adults=2&group_children=0&no_rooms=1&b_h4u_keep_filters=&from_sf=1&ss_raw=athens+Greece&ac_position=0&ac_langcode=en&ac_click_type=b&dest_id=-814876&dest_type=city&iata=ATH&place_id_lat=37.975659&place_id_lon=23.734866&search_pageview_id=79a1858a27bb0013&search_selected=true) | Used for the marker and the text content for a place to stay in Athens
 9 | https://www.planetware.com/tourist-attractions-/athens-gr-ath-ath.htm | Used for the marker and the text content for the Acropolis in Athens
 10 | https://www.foodieflashpacker.com/restaurants-in-tbilisi/ & https://www.facebook.com/sulicowinebar/ | Used for the content of the marker for a place to eat in Tbilisi
 11 | [Booking.com](https://www.booking.com/hotel/ge/bricks-room.en-gb.html?aid=318615;label=New_English_EN_GBIE_5496343105-o3H%2ArANRilZd5LRixj8tfwS217246569576%3Apl%3Ata%3Ap1%3Ap2%3Aac%3Aap%3Aneg%3Afi16483151479%3Atiaud-297601666475%3Adsa-55482331735%3Alp1006965%3Ali%3Adec%3Adm;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the place to stay marker for Tbilisi
 12 | https://www.saltinourhair.com/georgia/tbilisi-georgia/ | Used for the marker content for the Sulphur Baths in Tbilisi
 13 | https://www.timeout.com/vienna/restaurants/best-restaurants-in-vienna | Used for the marker for a place to eat in Vienna
 14 | [Booking.com](https://www.booking.com/hotel/at/grand-wien.en-gb.html?aid=377399;label=vienna-emzYuM5MFtKA0DtbD2zHFQS286619947823%3Apl%3Ata%3Ap11240%3Ap2%3Aac%3Aap%3Aneg%3Afi%3Atiaud-297601666475%3Akwd-269876017%3Alp1006965%3Ali%3Adec%3Adm%3Appccp%3DUmFuZG9tSVYkc2RlIyh9YX-SVbABBf1_4WBEGJjkaYE;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the place to stray in Vienna
 15 | https://www.timeout.com/vienna/things-to-do/best-things-to-do-in-vienna | USed for the marker content for Wiener Riesenrad in Vienna
 16 | https://www.timeout.com/lisbon/restaurants/lambrettazzurra-pizzeria & https://www.facebook.com/LambrettazzurraPizzeria | Used for the marker for a place to eat in Cascais
 17 | [Booking.com](https://www.booking.com/hotel/pt/albatroz.en-gb.html?aid=356980;label=gog235jc-1DCAMouwFCB2Nhc2NhaXNICVgDaFCIAQGYAQm4ARfIAQzYAQPoAQH4AQKIAgGoAgO4AuLg_P4FwAIB0gIkMjRhYzM0OTItNTI4ZC00M2U0LTk4YTgtNjYyYTk4MmMxNGVj2AIE4AIB) | Used for the marker for a place to stay in Cascais 
 18 | https://www.thecrazytourist.com/15-best-things-cascais-portugal/ | Used for the marker for Boca do Inferno in Cascais
 19 | https://travelaway.me/sibiu-best-restaurants/ & http://www.jules-restaurant.ro/ | Used for the marker for a place to eat in Sibiu
 20 | [Booking.com](https://www.booking.com/hotel/ro/t-house.en-gb.html?aid=373411;label=city-sibiu-WbeAxHHByzgog2J8%2AvSNugS383257674361%3Apl%3Ata%3Ap1%3Ap2%3Aac%3Aap%3Aneg%3Afi%3Atiaud-261710242742%3Akwd-1520443560%3Alp1006965%3Ali%3Adec%3Adm%3Appccp%3DUmFuZG9tSVYkc2RlIyh9Ybz4KBg0DTFCTn0pIbYiAXw;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the marker for a place to stay in Sibiu
 21 | https://www.thecrazytourist.com/15-best-things-to-do-in-sibiu-romania/ | USed for the marker for the Bridge of Lies in Sibiu
 22 | https://www.lonelyplanet.com/belgium/wallonia/namur/restaurants | Used for the marker for a place to eat in Namur
 23 | [Booking.com](https://www.booking.com/hotel/be/ms-elisabeth.en-gb.html?aid=373411;label=namur-eyPh_eYwT2HGVg6oHnEeWgS406089779927%3Apl%3Ata%3Ap1%3Ap2%3Aac%3Aap%3Aneg%3Afi%3Atiaud-297601666475%3Akwd-1486720022%3Alp1006965%3Ali%3Adec%3Adm%3Appccp%3DUmFuZG9tSVYkc2RlIyh9Ybz4KBg0DTFCTn0pIbYiAXw;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the marker for a place to stay in Namur
 24 | https://www.planetware.com/tourist-attractions-/namur-namen-b-nm-nn.htm | Used for the marker for the Church of Notre Dame and Treasury in Namur
 25 | https://theculturetrip.com/europe/croatia/articles/the-10-best-restaurants-in-rijeka/ & http://restoran-lovorka.incroatia.info/en/kontakt.html | Used for the marker for a place to eat in Rijeka
 26 | [Booking.com](https://www.booking.com/hotel/hr/apartments-porto-marina.en-gb.html?aid=373411;label=rijeka-QkYM0Th6F%2AyCLDTulsFlpwS388389303072%3Apl%3Ata%3Ap1%3Ap2%3Aac%3Aap%3Aneg%3Afi%3Atiaud-297601666475%3Akwd-1630451870%3Alp1006965%3Ali%3Adec%3Adm%3Appccp%3DUmFuZG9tSVYkc2RlIyh9Ybz4KBg0DTFCTn0pIbYiAXw;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the marker for a place to stay in Rijeka
 27 | https://www.planetware.com/tourist-attractions-/rijeka-hr-kv-r.htm | Used for the marker for the Capuchin Church of Our Lady of Lourdes in Rijeka
 28 | https://www.timeout.com/paris/en/restaurants/the-100-best-restaurants-in-paris | Used for the marker for a place to eat in Paris
 29 | [Booking.com](https://www.booking.com/hotel/fr/les-2-girafes.en-gb.html?aid=377399;label=paris-uIHbvGhhHoK3x6LyNz17SwS382902578055%3Apl%3Ata%3Ap14260%3Ap2%3Aac%3Aap%3Aneg%3Afi%3Atiaud-297601666475%3Akwd-269911447%3Alp9046392%3Ali%3Adec%3Adm%3Appccp%3DUmFuZG9tSVYkc2RlIyh9YX-SVbABBf1_4WBEGJjkaYE;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the marker for a place to stay in Paris
 30 | https://www.fodors.com/world/europe/france/paris/experiences/news/photos/20-ultimate-things-to-do-in-paris | Used for the marker for the Eiffel Tower in Paris
 31 | https://theculturetrip.com/europe/poland/articles/the-best-restaurants-in-bydgoszcz-poland/ | Used for the marker for a place to eat in Bydgoszcz
 32 | [Booking.com](https://www.booking.com/hotel/pl/apartament-bydgostia.en-gb.html?aid=830766;label=bydgoszcz-2mpt6CYW3fQ0bmQFKwdJhQS382784749321%3Apl%3Ata%3Ap1%3Ap21%2C093%2C000%3Aac%3Aap%3Aneg%3Afi%3Atiaud-297601666475%3Akwd-11563970092%3Alp1006965%3Ali%3Adec%3Adm%3Appccp%3DUmFuZG9tSVYkc2RlIyh9YRfRdUUL2hDPeOc6GIaLzvI;sid=8f5d6c7740e4b688a551571a0ae3738e) | Used for the marker for a place to stay in Bydgoszcz
 33 | https://www.thecrazytourist.com/15-best-things-to-do-in-bydgoszcz-poland/ | Used for the marker for the Museum of Soap and Dirt in Bydgoszcz
 
 
### Media

No. | URL | Copyright | Used for
--|--|--|--
1 |https://www.tajtravel.com/blog/wp-content/uploads/2019/07/travel-europe-places.jpg |No Copyright information was availiable | The main image on the page before a destination is selected
2 |  https://www.europeanbestdestinations.com/european-best-destinations-2020/  | Matthieu Cadiou / European Best Destinations | Used for the image for the Calmar section
3 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Anastasios71 | Used for the image for the Athens section
4 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Boris Stroujko | Used for the image for the Georgia section
5 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Christian Stemper / Vienna.info | Used for the image for the Vienna section
6 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Visit Cascais | Used for the image for the Cascais section
7 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | sibiucity.ro | Used for the image for the Sibiu section
8 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Denis Erroyaux / Visit Namur | Used for the image for the Namur section
9 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Rijeka Tourist Board | Used for the image for the Rijeka section
10 | https://www.europeanbestdestinations.com/european-best-destinations-2020 | Ekaterina Pokrovsky | Used for the image for the Paris section
11 | https://www.europeanbestdestinations.com/european-best-destinations-2020/ | Visit Bydgoszcz | Used for the image for the Bydgoszcz section

### Acknowledgements

 * I received inspiration for the colour scheme using the colour scheme creator: [Coolors.co](https://coolors.co/)

 * My mentor Antonio Rodriguez who has provided me with guidance and support through the project