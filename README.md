# -SEI-Project-Two

Working with APIs is a very exciting part of this project, it was very interesting to figure out how some free APIs worked and the type of data they were bringing back.
My partner and I took some time trying to find one we both liked,  and settled on the NASA Picture of the Day API.

Wireframing for this project didn’t take us too long and we quickly settled on writing 4 main pages for our MVP : Home, all pictures, show pictures and a picture of the day.
Our additional features included filtering by month and year and for the user to have the ability to search by title, and have a pick a date page, where we could pass down a date parameter using a form


The main challenge we faced using this api for our AllPictures page was changing the dates inside our get request using pieces of states. The idea behind it was that whenever the user selects another month, or types something the page rerenders and filters through images accordingly.

Working on picture of the day and Home were the faster components, as it was either just displaying a hero container or making one get request.


The pick a date feature was very interesting and did require us to think of the most optimum way to indicate to the user what the best date format was, and upon submitting the button we would pass the date as a parameter for our next component.
The Show picture and show your picture component are both using a third child component as we found it was a good way not to repeat our code and make that component reusable.

We spent most of our time left working on our css, and trying to use bulma and css was very complex since bulma does use some set css when we apply one or more classes to elements, so we found out using dev tools on browser worked best for us when writing our css.
