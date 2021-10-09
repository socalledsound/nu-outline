## React Course Outline week 4

# OLD STUFF TO KEEP

    I think the intro to MVC and flux and redux overview is important but I'd like to do it somewhat differently
    intro to redux exercise will be different.

# week 4 REDUX

#### v0 let's brush up on functions

    -- show them something like
        (() => (()=>) =>)()
    -- functions are first class citizens
    -- functions can be passed into functions
    -- functions can be partially applied and curried
    -- sum(2)(3)

##### v1 3-5 mins WHY REDUX

    Why Redux?
        -- FIRST, you don't always need redux.  Abramov quote.
        -- when are some times you might need redux?  USERS.
        -- this app doesn't really need redux but you have to start small to learn
        -- redux is actually SO SMALL and so focused, once you understand it, you'll realize it's not that big of a deal
        -- what's hard, actually, is state management

##### v2 3-5 mins WHAT IS REDUX

What is redux?
-- what is an application and how is it different from a website?
-- seperation of concerns: seperate out the VIEW aka side effects
-- different architectures - MVC, FLUX (position flux within functional paradigm)
(should I mention smalltalk? I'd like to try but might cut it)
https://medium.com/@garychambers108/understanding-flux-f93e9f650af7
flux
-- VIEW -> DISPATCH -> ACTION -> STORE -> VIEW
-- (also, REDUCER, which is part of the store)
-- SINGLE SOURCE OF TRUTH

## now we tackle each one of those things, start with REDUCER but first, let's understand Array.reduce() and understand what it has to do with redux.

#### v3 7.5 mins ARRAY.REDUCE (should this go before redux intro?)

    Array.reduce()
    SCARY!  But amazing.
    Canonical example of summing.
    This has nothing to do with redux, right?
    But what if we apply this idea to the notion that we want a single state object?
    ie we use reduce to immutable update our single state object?
    one more example, where we return an object
    THE REDUCER IS THE FUNCTION YOU PASS IN TO REDUCE

#### v4 3-5 mins Small Redux App (this will be several videos)

    PROJECT: build a small app
    Drawing app (or likable images app???  drawing app has less setup)
    First video let's do the VIEW
        -- make a ball component that follows the mouse
        -- store an array of balls and render them
        -- what if we want to save a drawing??!?!?!
        -- let's add a save drawing button.
        -- but where do we show this?
        -- let's add a new page where we see all of the drawings but smaller
        -- but how do we connect these things?  and what if we have multiple users?  I think we might could need redux.
        -- let's add a store

##### v5 3-5 mins STORE

    THE STORE
        -- is the single source of truth, the god dream.
        first let's look at what a store actually is
        -- dispatch
        -- getState

    now let's build it with redux.  we pass in a reducer to configureStore and we're done.
    but oh shit, we need a reducer

#### v6 3-5 mins REDUCER

    -- ok so we know a reducer is the function we pass in to Array.reduce.
    -- why do we need a reducer again?  let's look at what that dispatch method of our store does
    -- (acc, cur) becomes (state, action)
    -- (and we can also pass in an initial state)
    -- make the reducer, which will add a sketch to a list of sketches when it receives the appropriate action.
    -- oh shit we need an action

#### v7 ACTIONS

#### v8 DISPATCH

        DISPATCH
        https://dev.to/dustinmyers/what-even-is-a-dispatch-function-27ma
        UseDispatch()

#### v9 SELECTORS

        -- but how do we get our data?
        -- useSelector()

#### v10 SLICES (should this go before actions?)

    -- if here, after introducing the characters, then refactor
    -- else if earlier then refactor just means moving the reducer
    -- also have a userslice here?

##### v 10.5 we need a PROVIDER

#### v11 let's start implementing this in our nucampsite: store and provider

    -- hard coded data
    -- let's start with the Provider and a store

#### v12 nucampsite slices : campsitesSlice

    -- campsitesSlice
    -- bring our filter from before into our slice as a selector

-- slice for each of campsites, comments, partners and promotions

#### v13 nucampsite selectors

### workshop:

    create a userSlice in the nucampsite
    show user avatar in header (can we use a picture of a unicorn please?)
    if clicked after login display user info in modal
    utilize the user on the comments page
    (finish by setting the user in initial state so we don't have to log in every time)
    (it would be cool to come back to this in the node course....)
