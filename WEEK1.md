## React Course Outline week 1

# approx how many minutes of videos per week????

currently two sections, 8 vids and 5 vids
i have approx 17 below, in three sections

##### old week 2 material:

123 can probably be mostly kept, just updated -- and perhaps expand a bit
keep 4 vscode thing
7 reactstrap - update

CHALLENGES ALL CLASS BASED
challenge : jsx and state
challenge : constructing lists - i
challenge : passing props - party time.

challenge: object destructuring from week 3

### week 1 : introduction to react

##### hello and welcome to the course - 1 short video

    just a welcome video and overview in broad terms, 1 minute

##### React Without React -- 2 c 7.5 minute videos?

    PROJECT: hi there : https://github.com/socalledsound/hi-without-react
    JS: DOM manipulation
        -- look at the index.html.
        -- getElement, createElement, element properties, appendChild
        -- we use camelCase when manipulting DOM properties with javascript
        -- React provides us with a thing called JSX, which we'll see in a bit, which is basically a shorthand for writing this kind of code
        -- React also has an important idea called the virtual DOM, which we'll explore in a bit.

    JS: FUNCTIONS
        arrow functions are cool
        functions should do one thing
        functions can have parameters, and default parameters too
        functions have a single return value; if we want to return more than one thing
            we can use an object or an array
        react components are always functions that return a single DOM element
        this render function is a lot like something you're about to see in React,
            except that it is diffing the 'real' DOM against the virtual DOM.

##### Getting Started With React right now looks like 10-12 10 min videos (is that too many!!!??)

    PROJECT: react Heartz:
    environment setup.  node.  node version manager?
    do we want to also have a video on npm, github, and the node_modules folder?
    (CODE CHALLENGE HERE??? deleting and bringing back node modules folder?)
    (CODE CHALLENGE ON GIT AND BRANCHES??)
    GIT/GITHUB/BRANCHES/HOW TO USE THESE REPOS
    perhaps even before we CRA, they download the github repo for the hearts and install it that way, run it and see it in action, then ask them to delete it and build it from scratch.
    CRA.
    Index.js
        - ReactDOM.render() (I'd like to ask them to delete everything in the source folder!  and rewrite it from scratch)
        - How the virtual DOM works
        - also mention that more broadly most node projects, not just React, start at an index.js
    COMPONENTS.
        -- overview.
        -- breaking a page down into its elements
        -- look at heart as a square and two circles.
        -- before we continue let's make sure we understand imports and exports
    JS: import and export ( CODE CHALLENGE HERE)
    App Component (will just be a container)
        --write the app and export it then import it.
        -- JSX
        -- PROPS
    JS: object AND ARRAY destructuring (CODE CHALLENGE HERE)
        -- remember how functions have a single return value?
        -- object and array destructuring comes in really handy here!
    feature folder: Heart
        -- give the heart a position
        -- props
    components folder: Circle, Square
        -- Circle, Square
    JS: Array Methods: Array.map()
    JS: implementing our own Array class to understand Array.map()
        -- and also this gives us a leg up on the class components when we get around to it
        --    map(cb){
                const arr = []
                for(let i = 0; i<this.length; i++){
                arr.push(cb(this.data[i], i))
                }
                return arr
            }
    Using Map in our Hearts App to make a bunch of hearts
        -- leave them with a challenge to take a getRandomColor function and make the hearts all have random colors.
    Challenge answer

##### Starting the Nucamp Project looks like 2-3 7.5 min videos to me?

    Overview:  let's look at animage of the finished site home page and try to understand it as components.
    CRA
    delete the source and start over, writing out index.js and App.js

#

    REACTSTRAP - video or just instructions?

#

    create the folders we'll eventually need:
        --app - 'shared' folder.  show them the data right off the bat.
            -- maybe a whole video talking about data somewhere????
        --assets (can we import images as files into our app instead of pulling them in as URLs?)
            -- maybe a video on importing images into react somewhere?
        --components
        --features
        --pages
        --utils
        -- we won't have anything in them yet.

#

    create the App component
        -- css className

#

    ACTUALLY I THINK THIS COMES IN WEEK3?
    create CampsiteDirectoryPage

## workshop week 1:

    create features/campsite, create CampsiteList and CampsiteCard, use map to make the list,
    and bring it in to the App.
    work on the header and the footer a bit
