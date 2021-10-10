## React Course Outline week 3

from old week 4

    computed property names and spread syntax
    (ternary was week 2)
    regex
    i think leave out controlled vs uncontrolled forms??
    instead maybe introduce a custom hook useForm?
    there is the toggling modals challenge...?

##### animation ++ formik (++ custom hook?)

LET'S DO MORE WITH ANIMATION:
2 options on main home page - one with a fade/slide - one with a carousel transition

fwiw react-spring install seems to work fine with yarn add, while npm requires --legacy-peer-deps or some fiddling
-- (this might ultimately be a great reason to skip animation
libraries entirely and just use css with custom hooks? but for now let's use spring)
--(Motion aka framer motion might be closer to formik fwiw, they do namecheck it in the formik docs...we can switch to this if you want to, it's mostly pretty similar)
-- i'd like to explain how all of these css animation libraries work first.

### animation

#### v1 first: a bit more on css in react

    -- react and css
    -- classNames with css file
    -- classNames with module.css file
    -- css in JS
        -- style prop with style object
    -- should we make a recommendation here?
    -- i think modules are gaining steam, personally, and I like them.

#### v2 using ternaries to conditionally render styles

    -- this kind of 'local' state is where useState really shines
    --[toggle, setToggle] = useState(false)
    -- <button onClick(() => setToggle(!toggle)) style={{backgroundColor: toggle ? 'red' : 'grey'}}>click me </button>
    or
    -- <button onClick(() => setToggle(!toggle)) className={toggle ? 'red' : 'grey'}>click me </button>
    -- but what if we want to transition from one color to another?  let's use css animations
    -- let's add a little jiggle to our FA heart

#### v3 review of how css animations work

    -- two different states
    -- keyframes

#### v4 animate on page load using useEffect()

#### v5 animate on toggle using useEffect() with dependencies

#### v6 animating with useSpring()
    -- gives us 'pysics-based' animations 
    -- what does that mean? easing curves.
    -- also, it's bomb easy to use and has a lot of advanced features, too
    -- let's use it for a bounce animation
    -- so now you know quite a bit about animation, let's apply it to our site
#### v7 let's animate the loading of our home page

    -- animated menu feature
        -- featured items (still hard coded data at this point)



start with a simple custom hook that chooses the animation component to render

Fade In card with useTransition()

# see how much time just the formik takes up here

    <!-- SIDE PROJECT: log in user useForm hook ?

#

#### v8 FORMS with Formik - 1 - html form review
    -- form
    -- input with id, name, type, onChange, value
    -- submit button
    -- but how do we update the value with the things the user types?
    -- we could use useState like this....
    -- but this will get complicated fast
    -- one idea is to make a custom hook -- i;ll show you how to do that later if you like but
    -- the easy choice is a library like Formik

# are we using the Formik hook or the component?

    -- if using the component then maybe we start with our own custom hook?
    -- or with the useFormik version like in the docs 

#### v9 formik 2 : useFormik
    -- useFormik is a hook which returns a formik object with keys for 
    values, handleChange and handleSubmit
    --let's add the values and handleChange to our form now
    -- now what about handleSubmit?  let's do that in the next video
#### v10 handleSubmit + computed property names

#### v11 validation : 
    -- do we want to keep our own validation or use Yup?
    -- people get irritated about regex and yup seems pretty easy


#### v12



    JS: SPREAD SYNTAX -- ??? what was that for in the old version?
    JS: COMPUTED PROPERTY NAMES
    JS: REGEX -- or use yup


    FORMIK




    -- useform hook ?

### week 3 workshop:

comments form
just log it to the console for now

    extra content:

https://blog.logrocket.com/the-top-5-react-animation-libraries-compared/
https://www.youtube.com/watch?v=kT6yYSwK1oA
https://codesandbox.io/s/xenodochial-buck-k40bj?file=/src/index.js:713-894
https://atheros.ai/blog/fade-in-and-fade-out-animation-with-spring-and-transition-react-hooks
https://react-spring.io/hooks/use-transition
https://codesandbox.io/s/0-intro-p8fsf?file=/src/App.js:296-338
https://css-tricks.com/making-sense-of-react-spring/

https://dev.to/ekeijl/simple-react-fade-animation-hook-5dp8
