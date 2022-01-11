# SEI Project Two - Astronomy Pictures


[Link](https://astronomy-pictures.netlify.app/)

<br/>

***Project Members***

[Mariana Lozynska](https://github.com/mlozynska)

<br/>

***Timeframe***

48 hours

<br/>


***Brief***

Build a React front-end application using React and a third party API.

<br/>


***Overview & Concept***

This group project is an app that uses the NASA API to display pictures uploaded by NASA in 2021, with an option to pick your own date and browse the picture for that day.

<br/>

***Technologies used***

- React
- JavaScript
- Axios
- Bulma
- CSS
- React Router Dom

<br/>
<br/>

***Approach Taken***

**Planning:**

Working with APIs is a very exciting part of this project, it was very interesting to figure out how some free APIs worked and the type of data they were bringing back.
My team member and I took some time trying to find one we both liked, and settled on the [NASA Picture of the Day API](https://apod.nasa.gov/apod/astropix.html).

<img width="1440" alt="Screenshot 2021-12-23 at 14 44 03" src="https://user-images.githubusercontent.com/69866434/148947241-e6753d71-2bbf-4a2a-9f9b-c4e3314f1778.png">


Wireframing for this project didn’t take us too long and we quickly settled on writing 4 main pages for our MVP : Home, all pictures, show pictures and a picture of the day.
Our additional features included filtering by month and year and for the user to have the ability to search by title, and have a pick a date page, where we could pass down a date parameter using a form.

<br/>

**Front-end:**

For the whole project, we pair coded so that each group member could have a say and understanding of all components.

<br/>
*AllPictures*
The main challenge we faced using this api for our AllPictures index page was building the filter, changing the dates inside our get request using pieces of states. The idea behind it was that whenever the user selects another month, or types something the page rerenders and filters through images accordingly.
Our initial useEffects loads the pictures from a set month, and the filter function (handleChange) will change the startMonth and endMonth every time a user selects a new month

<br/>

useEffect function:

<img width="158" alt="Screenshot 2021-12-23 at 14 50 07" src="https://user-images.githubusercontent.com/69866434/148947358-1d547198-9e0d-41cf-822a-9701a8791b60.png">

<img width="1072" alt="Screenshot 2021-12-23 at 14 52 45" src="https://user-images.githubusercontent.com/69866434/148947394-2fa68f8b-c46b-4502-9473-db00cbaeba78.png">

<br/>

Filter function:

<img width="442" alt="Screenshot 2021-12-23 at 14 49 15" src="https://user-images.githubusercontent.com/69866434/148947457-5da2da86-2be9-47c6-8948-c9a001bd98a1.png">


Working on pictures of the day and Home were the faster components, as it was either just displaying a hero container or making one get request.

<br/>
<br/>

*Pick a Date*

The pick a date feature was very interesting and did require us to think of the most optimum way to indicate to the user what the best date format was, and upon submitting the button we would pass the date as a parameter for our next component.

<br/>

Code on ‘ChooseDate’ component:

<img width="366" alt="Screenshot 2021-12-23 at 14 55 28" src="https://user-images.githubusercontent.com/69866434/148947564-c0cc00ba-6c12-46ca-9d33-8f67a8d17279.png">

<br/>

Route:

<img width="588" alt="Screenshot 2021-12-23 at 14 56 46" src="https://user-images.githubusercontent.com/69866434/148947637-7fc8d9de-61de-4f1d-996b-1f6c46bd72b7.png">

<br/>

Extracting parameters from component displaying at ‘ShowYourPicture’

<img width="254" alt="Screenshot 2021-12-23 at 14 55 06" src="https://user-images.githubusercontent.com/69866434/148947668-3d41ae5e-558d-48b7-9dea-fb75f3a01978.png">

The Show picture and show your picture component are both using a third child component as we found it was a good way not to repeat our code and make that component reusable.

<br/>
<br/>

**Styling**

We left styling at the end, and decided to use Bulma and some CSS. Our design idea was fairly simple, and the main layout we wanted to get right was displaying all pictures in the index page with the same height. We were able to do this using the bulma classes for image size(‘image is-5by4’)

<br/>

Before:

![Screenshot 2021-10-27 at 09 37 41](https://user-images.githubusercontent.com/69866434/148947972-edd41fb8-921d-434e-9d7e-5543178c088c.png)

<br/>

After:

<img width="1437" alt="Screenshot 2021-10-28 at 18 51 03" src="https://user-images.githubusercontent.com/69866434/148947985-403c6f65-9260-4365-9997-a68157e3905f.png">

<br/>
<br/>

**Some features I would have liked to add include:**

- More filters for the user (for example year or day).
- Responsive design.

<br/>

**Wins:**

- We were able to successfully use the NASA picture api and exploiting it for multiple uses in the app.

<br/>

**Challenges:**

- Extracting the right images was a challenge, especially because it took time to load, this is why we had to filter by month on the index page.

<br/>

**Known bugs:**

- The website will, by default, show pictures from 2021.
- The oldest photo dates back to June 16 1995, however this is not mentioned anywhere.

<br/>

***Key learnings***

This project taught me how to pair code effectively, as well as exploiting an API to its fullest. We did have some difficulty setting it up because it needed a key, and that came with its own challenges. We realized the dates also needed to be in a specific formatting, since they would be directly embedded in our get request URL. 


