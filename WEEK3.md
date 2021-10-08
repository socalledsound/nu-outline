## React Course Outline week 3

from old week 4

    computed property names and spread syntax
    (ternary was week 2)
    regex
    i think leave out controlled vs uncontrolled forms??
    there is the toggling modals challenge...?

##### animation ++ formik

LET'S DO MORE WITH ANIMATION:
2 options on main home page - one with a fade/slide - one with a carousel transition

fwiw react-spring install seems to work fine with yarn add, while npm requires specifying peer dependencies and praying.
-- (this might ultimately be a great reason to skip animation
libraries entirely and just use css with custom hooks? but for now let's use spring)
--(Motion aka framer motion might be closer to formik fwiw, they do namecheck it in the formik docs...)

### animation

    -- react and css
        -- style prop
        -- classNames with css file
        -- classNames with module.css file


    -- animated menu feature
        -- featured items (at this point they're coming down
        as props from the App)

    -- CHALLENGE -- make the buttons and a toggle using useState
    -- challenge answer
    -- two options, for now one just says carousel
    -- the other one, we build:
        -- introducing react spring

start with a simple custom hook that chooses the animation component to render

Fade In card with useTransition()

    extra content:

https://blog.logrocket.com/the-top-5-react-animation-libraries-compared/
https://www.youtube.com/watch?v=kT6yYSwK1oA
https://codesandbox.io/s/xenodochial-buck-k40bj?file=/src/index.js:713-894
https://atheros.ai/blog/fade-in-and-fade-out-animation-with-spring-and-transition-react-hooks
https://react-spring.io/hooks/use-transition
https://codesandbox.io/s/0-intro-p8fsf?file=/src/App.js:296-338
https://css-tricks.com/making-sense-of-react-spring/

https://dev.to/ekeijl/simple-react-fade-animation-hook-5dp8

    <!-- SIDE PROJECT: log in user useForm hook ?
    JS: SPREAD SYNTAX
    JS: COMPUTED PROPERTY NAMES
    JS: REGEX --


    FORMIK


    -- useform hook ?

week 3 workshop:
comments form
just log it to the console for now
