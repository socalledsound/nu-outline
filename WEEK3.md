## React Course Outline week 3

# NOTE/QUESTION

    -- in formik docs they teach formik by starting with the useFormik hook as I've done here,
    which does I think help students understand what it is that formik is doing?
    but we could also skip that step if we feel pressed for time.

    -- ALSO they use Yup.  Do we want to use that?  Would eliminate need for regex but also
    eliminate that teaching opportunity.

from old week 4

    computed property names and spread syntax
    (ternary was week 2)
    regex
    i think leave out controlled vs uncontrolled forms??
    but instead discuss the difference between the component and hook models
    there is the toggling modals challenge...

##### animation ++ formik (++ custom hook?)

    IN WEEK 5 animation will be continued with 2 options on main home page -
    - one with a fade/slide
    - one with a carousel transition
    but for now just the one option

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

#### v2 ternary operator

#### v3 using ternaries to conditionally render styles

    -- this kind of 'local' state is where useState really shines
    --[toggle, setToggle] = useState(false)
    -- <button onClick(() => setToggle(!toggle)) style={{backgroundColor: toggle ? 'red' : 'grey'}}>click me </button>
    or
    -- <button onClick(() => setToggle(!toggle)) className={toggle ? 'red' : 'grey'}>click me </button>
    -- but what if we want to transition from one color to another?  let's use css animations
    -- let's add a little jiggle to our FA heart

#### v4 review of how css animations work

    -- two different states
    -- keyframes
    -- timing functions
    -- we need access to component life cycle methods

#### v5 useEffect() probably longish, 10 mins?

    -- side effects
    -- component life cycle methods
    -- dependencies
    -- cleanup

#### v6 animate on toggle using useEffect() with dependencies

    useEffect(() => {
    renderAnimations()
    }, [toggle])
    const renderAnimations = () => {
    return toggle ? setAnimation(1) : setAnimation(0)
    }

#### v7 animating with useSpring()

    -- gives us 'pysics-based' animations
    -- what does that mean? easing curves.
    -- also, it's bomb easy to use and has a lot of advanced features, too
    -- let's use it for a bounce animation
    -- so now you know quite a bit about animation, let's apply it to our site

#### v8 let's animate the loading of our home page

    -- animated menu feature
        -- featured items (still hard coded data at this point)

start with a simple custom hook that chooses the animation component to render

Fade In card with useTransition()

# see how much time just the formik takes up before thinking about this other thing

    <!-- SIDE PROJECT: log in user useForm hook ?

#

#### v9 FORMS with Formik - 1 - html form review (building login form)

    -- form
    -- input with id, name, type, onChange, value
    -- submit button
    -- but how do we update the value with the things the user types?
    -- we could use useState like this....
    -- but this will get complicated fast
    -- one idea is to make a custom hook -- i;ll show you how to do that later if you like but
    -- the easy choice is a library like Formik
    -- we can use formik either as a hook or as a component, we'll show you both here but ultimately use the component

#### v10 formik 2 : useFormik (less than 5 minutes)

https://formik.org/docs/tutorial
-- useFormik is a hook which returns a formik object with keys for
values, handleChange and handleSubmit
--let's add the values and handleChange to our form now
-- and we can also add a handleSubmit function that is called on submit
-- but how does handleChange work? Let's take a look. but first lets understand computed property names

#### v11 computed property names (5 minutes?)

JS: COMPUTED PROPERTY NAMES

#### v12 SPREAD SYNTAX updating an array or object with useState

    const [items, setItems] = useState([]);
     setItems([
      ...items,
      {
        id: items.length,
        name: itemName
      }
    ]);

#### v13 prevState

    import React, { useState } from 'react';

    function Counter() {
    const [count, setCount] = useState(0);

    function increment() {
    setCount(prevState => prevState + 1);
    }

    return (

    <div>
    the count is: {count}!
    <br />
    <button onClick={increment}>
    increase count
    </button>
    </div>
    );
    }

#### v13 handleChange

    https://formik.org/docs/tutorial
    (from the link above)
    // initialize values to empty object
    const [values, setValues] = React.useState({});
    //
    const handleChange = event => {
    setValues(prevValues => ({
    ...prevValues,
    // we use the name to tell Formik which key of `values` to update
    [event.target.name]: event.target.value
    });
    }

#### v15 validation with yup OR regex:

    -- do we want to keep our own validation or use Yup?
    -- people get irritated about regex and yup seems pretty easy
     -- if regex need a video or two on regex
     -- students are consistently frustrated by the regex materials

#### v16 Formik Components

    -- formik components use Context
    -- should we explain useContext here?
    -- let's build the

#### v16 Building the Contact Form probabkly 10 mins

    ( maybe 2 5 min videos is better but not sure where it breaks down)
    -- Formik, pass in initialValues, onSubmit and validate
    -- use Form, Field and ErrorMessage
    -- write the handleSubmit function

#### v17 optional: useField for re-usability and composability

### week 3 workshop:

#### comments feature - did we make this yet?? when? should we just do all the comments stuff here?

TOPICS FOR REVIEW:

    OLD:
    task 1: ComentForm component with a modal and a reactstrap Button
         -- should we be showing them how to make a useModal component in this course?
        -- it would be nifty but maybe too much
    task 2: make the form with Formik, Form, Field, ErrorMessage
    task 3: form validation

    NEW COULD BE (if we don't do comments elsewhere):
    task 1: make the comments feature folder.  make a CommentsList component, bring in the comments, then
        make the Comment component and render each of the comments.
    task 2: task 1 from above
    task 3: make the form with Formik (use yup for validation)

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
