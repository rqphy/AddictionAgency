# Addiction Agency

/!\ The code won’t be displayed because it’s a private project.

## The idea

![Homepage Addiction Agency](https://juq1maqrjs.ufs.sh/f/r1m4dnkvsK4QVQdoEFbODc6AFL2QrJse1TYB7lZEUChMkiSI)

The website will be a single page with a controlled scroll. There will be 3 parts:

- Works, you’ll be able to find all of their creations. Each frame will have a video in the background, the name of the project and the client brand. Some project won prices that need to be displayed.
- About, you’ll understand what and who is Addiction Agency.
- Contact.

[Live](https://www.addiction-agency.com/)

## Some issues

### Custom scroll system

I couldn’t find any complete and editable library to do the controlled scroll. Let’s create it in native Javascript. The first thing to do is to create a variable where I’ll stock the scrollY value. Then, I add the scroll event listener where I can compare the current scrollY and the variable I just created.

There will be 2 cases:

- The value is negative. In this case, the user scrolled down.
- The value is positive. You get it, the user went up.

I’ll set the body in overflow hidden and update the transform value on the main element. It basically is a vertical carrousel.

### Performances

The high number of projects translate by a high number of videos. Performance wise it’s usually a bad idea to load multiple videos at the first load. I needed to ask for lower quality videos for mobile. The website is still slow, that should be the main focus for the next website update.
