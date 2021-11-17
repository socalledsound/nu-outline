# TODO

    BRING GIT AND GITHUB BACK IN -- very difficult to get help without it.
    note which are big picture and which are exercise

# nucamp react course rewrite outline, one page for each week

## overview:

## week1 : introduction to react

##### PART 1 : react without react

    1: welcome to the course, react is cool                        -- 2 mins
    2: react core principles -- 5 mins
    3. CORE JS - the DOM
    (constants?)
    4. r-w-r create and render element
    5. CORE JS -- functions of a higher order
    6. r-w-r -- Welcome Message, App and render
    7. CORE JS -- object destructuring
    8. r-w-r -- Welcome Message with props
    9. CORE JS -- template literals
    10. r-w-r -- Welcome Message as a template
    11. CORE JS -- Array methods: Array.map()
    12. r-w-r -- several welcome messages

    <!-- 13. Proxies
    7. environment setup -->

    <!-- 2-2 parts: react without react1: the non-virtual dom
    3-2 parts: react without react2: composing with functions
    3B also has template literals -->

<!--
    alt2: review: the DOM
    2: react x react 1: DOM manipulation with JS    -- 7.5 mins
    3: react x react 2: composing with functions    -- 7.5 mins -->

    4: environment setup                            -- 5 mins

<!-- ##### we don't need this here if we use moodle links

    5: leveraging git and github                    -- 10 mins -->

##### PART 2 React Hearts

    STARTS VIDEO 13 now
    ## react hearts/react ice cream/small app
    13: create react app                             -- 5 mins
    14: CORE JS : import export                                -- 5 mins
    15: ReactDOM                                     -- 5 mins
    16: Components                                   -- 7.5 mins
    17: CLASS components                             -- 7.5 mins
    18: App, Heart, Circle, Square components
    19. multiple Hearts
    <!-- 18: App Component                                -- 7.5 mins
    19: Object and Array destructuring               -- 5 mins
    20: Heart + Circle + Square PROPS                -- 10 mins -->
    <!-- Array Methods: Array.from and Array.map      -- 7.5 mins
    15 Understaning Array.map by building it        -- 10 mins -->
    <!-- 21 Using Array.map and Array.from to make random hearts  -->

##### PART 3 Nucamp Project (or should this just be in workshop>?)

    20 Starting the Nucamp Project: overview        -- 5 mins
    21 CRA the nucamp project                       -- 5 mins
    22 getting started with git and github
    23 Setting up file structure                    -- 5 mins
    20 Making the App component                     -- 5 mins

    extra material: git and github

    WORKSHOP
        TOPICS FOR REVIEW:
            -- functional javascript
            -- the dom and virtual dom
            -- object and array destructuring
            -- array methods
            -- classes
            -- components
            -- JSX
            -- props
            -- create-react-app
            -- file structure of a react app
        TASKS:
            task 1: create features/campsite, campsite List and campsite Card
            task 2: work on the header?
            task 3: work on the footer?

### week2: Hooks, State, Router

    1 what is a SPA?                            -- 3-5 mins
    2 What is React router?                     -- 3-5 mins
    3 react-router in our project               -- 7.5 mins
    4 header / links                            -- 10 mins
    5 footer links                              -- 5 mins
    6 subheader ( breadcrumbs)                  -- 5 mins
    7 HomePage                                  -- 5 mins
    8 About, Contact, Campsite Directory Pages  -- 10 mins
    9 Introducing Hooks                         -- 5 mins
    10 useState                                 -- 10 mins
    11 clickable heart with FA                  -- 5 mins
    12 useState on CampsiteDirectory page       -- 10 mins?
    13 Lifting State                            -- 10 mins?
    14 params + useParams                       -- 7 mins
    15 (*o) understand useState by building it  -- 10 mins

    WORKSHOP
        TOPICS FOR REVIEW:

        TASKS

### week3: animation ++ formik

    1 css in react                              -- 7 mins
    2 JS: ternary operator                      -- 5 mins
    3 conditionally rendering styles            -- 5 mins
    4 css animations overview/review            -- 5 mins
    5 useEffect                                 -- 10 mins
    6 animating on page load with useEffect     -- 5 mins
    7 animating with useSpring                  -- 5 mins
    8 AnimatedMenu feature                      -- 10 mins
    9 HTML Forms review                         -- 5 mins
    10 Formik: useFormik                        -- 5 mins
    11 JS: computed property names              -- 5 mins
    12 JS: spread syntax                        -- 5 mins
    13 accessing prevState                      -- 5 mins
    14 handleChange in useFormik                -- 5 mins
    15 validation REGEX or YUP???               -- 10 mins
    16 Formik components                        -- 5 mins
    17 building ContactForm                     -- 10 mins
    18 (*o) useField with Formik                -- 10 mins
    19 (*o) custom useForm hook                 -- 20 mins?

    WORKSHOP:
        TOPICS FOR REVIEW:
        TASKS:
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

### week4: REDUX

    1 a deeper dive into functions              -- 10 mins
    2 why redux?                                -- 5 mins
    3 redux background 1 MVC FLUX STATE MACHINE -- 5 mins
    4 redux background 2 local vs global state  -- 5 mins
    5 Array.reduce()                            -- 10 mins
    ## small redux app: drawing app
    ## this might be too much, but something simple
    6 View layer                                -- 10 mins
    7 Provider                                  -- 3 mins
    8 Store                                     -- 5 mins
    9 reducer                                   -- 7 mins
    10 Actions                                  -- 5 mins
    11 dispatch + useDispatch()                 -- 5 mins
    12 selectors + useSelector()                -- 5 mins
    13 slices                                   -- 5  mins
    14 slices in our app                        -- 10 mins
    ##
    15 nucampsite: provider and store
    16 nucampsite: campsitesSlice reducer
    17 campsitesSlice selectors
    18 nucampsite : other slices

    WORKSHOP"
        TOPICS FOR REVIEW:

        TASKS:

### week5

    1 JS review: callback functions
    2 JS PROMISES
    3 API call use fetch with useEffect
    4 thunks pt 1
    5 thunks pt 2
    6 createAsyncthunk
    7 fetchCampsites
    8 other slices async stuff
    9 updating our selectors
    10 handling isLoading states
    11 - 17 carousel

    WORKSHOP
        TOPICS FOR REVIEW:

        TASKS:

### appendix 1: javascript concepts

### appendix 2: react without react mach 2

### week 6 advanced topics for another course

    integration with a backend service
    sagas
    server side rendering
    useRef, useContext
    custom hooks
    children
    using SVG or Canvas
    web audio/middlewares
    react query + rtk query
    understanding immer
