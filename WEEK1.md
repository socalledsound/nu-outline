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

##### video 1 hello and welcome to the course - 1 short video

    just a welcome video and overview in broad terms, 1 minute

## React Without React -- 2 c 7.5 minute videos?

    I think in these two videos they are just looking at the code as we review,
    they don't need to build this.

#### video 2 react without react 1: DOM manipulation -- 7.5 mins?

    PROJECT: hi there : https://github.com/socalledsound/hi-without-react
    (talk them through this download onscreen)
    JS: DOM manipulation
        -- look at the index.html.
        -- getElement, createElement, element properties, appendChild
        -- we use camelCase when manipulting DOM properties with javascript
        -- React provides us with a thing called JSX, which we'll see in a bit, which is basically a shorthand for writing this kind of code
        -- React also has an important idea called the virtual DOM, which we'll explore in a bit.

#### video 3 composing with functions -- 7.5 mins?

        arrow functions are cool
        functions should do one thing
        functions can have parameters, and default parameters too
        functions have a single return value; if we want to return more than one thing
            we can use an object or an array
        there's actually a lot more to learn about functions in JS, but we'll come back to it
        react components are always functions that return a single DOM element, eg a div
        this render function is a lot like something you're about to see in React,
            except that in React we get that notion of a virtual DOM, which we'll talk about soon.

####

    PROJECT: react Heartz:

#### video 4 : Environment setup (is this a video or just a text page?) -- 5mins max

    node.  node version manager?
    yarn vs npm
    (--legacy-peer-deps? or just yarn?)
    git
    LOOKING AT YOUR TERMINAL FOR ERRORS

#### video 5 leveraging git and github -- probably 10 mins honestly

    why is git awesome?
    why is github also awesome?
    (CODE CHALLENGE HERE??? deleting and bringing back node modules folder?)
    (CODE CHALLENGE ON GIT AND BRANCHES??)
    GIT/GITHUB/BRANCHES/HOW TO USE THESE REPOS
    before we CRA, they download the github repo for the hearts and install it that way,
    run it and see it in action, then ask them to delete it and say that we'll build it from scratch,
    but they can refer to it if they get lost or confused.
    (should we also give them the code for the nucamp site somewhere?  this is a big question in my mind
    that I truly don't know the answer too, after 20 years of teaching -- is it better to trust them or not???)

#### video 6 CRA

    CRA.
    let's take a quick tour of what got installed
    and mention that there are templates
    eg --template redux

#### video 7 import export - 5 mins?

    the different ways to import and export
        -- named vs default
    import order is stylistically important
    JS: import and export ( CODE CHALLENGE HERE?)

#### video 8 ReactDOM - 5 mins?

    (I'd like to ask them to delete everything in the source folder!  and rewrite it from scratch)
    starting with Index.js
    - ReactDOM.render()
    - The virtual DOM
        -- Fiber
        -- reconciliation
        --
    - also mention that more broadly most node projects, not just React, start at an index.js

#### video 9 Components - 7.5 mins?

    COMPONENTS.
        -- overview.
        -- breaking a page down into its elements
        -- look at heart as a square and two circles.
        -- before we continue let's make sure we understand imports and exports

#### video 10 App (+ JSX) - 7.5 mins?

    App Component (will just be a container)
        --write the app and export it then import it.
        -- JSX

#### video 11 Heart + Circle + Square PROPS -- 10 mins

    -- pass the heart a position from the App
    -- then pass positions to the Circle and Square

#### video 12 Object and Array Destructuring -- 5 mins?

    destructure those props
    what is destructuring?
    -- remember how functions have a single return value?
    -- object and array destructuring comes in really handy here,
        as we'll find out when we get to hooks and redux!
    JS: object AND ARRAY destructuring (CODE CHALLENGE HERE?)

#### video 13 Array methods : Array.from() and Array.map() -- making a bunch of randomly placed hearts

    -- In our App, let's make an Array of random positions
    -- leave them with a challenge to take a getRandomColor function and make the hearts all have random colors.

#### video 14 classes in javascript

    -- a class is a special type of function that returns an Object.
    -- there's another way to create React components - as classes
    -- at one time these were very useful for managing the state of your application.
    -- now with hooks they are not recommended
    -- it's kind of a thing of the past but still a great thing to know about
    -- BUT - classes are still very much a thing in javascript and an important thing to know about!
    -- For instance, Array is a class.

#### video 15 Understand Array.map() by implementing our own array class (is this too much?)

    JS: implementing our own Array class to understand Array.map()
        -- and also this gives us a leg up on the class components when we get around to it
        --    map(cb){
                const arr = []
                for(let i = 0; i<this.length; i++){
                arr.push(cb(this.data[i], i))
                }
                return arr
            }

#### video 16 : Challenge answer

#

    REACTSTRAP - video or just instructions?

#

## video 16 : Starting the Nucamp Project 1: overview and intro

    Overview:  let's look at animage of the finished site home page and try to understand it as components.

## video 17 :

    CRA
    delete the source and start over, writing out index.js and App.js

## video 18 : file structure

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

## video 18 : what are features?

## video 20 : the App component

    create the App component
        -- css className

#

## workshop week 1:

    TOPICS:
        -- functional javascript
        -- the dom and virtual dom
        -- object and array destructuring
        -- array methods
        -- classes
        -- components
        -- JSX
        -- props
        -- create-react-app



    create features/campsite, create CampsiteList and CampsiteCard, use map to make the list,
    and bring it in to the App.
    work on the header and the footer a bit
