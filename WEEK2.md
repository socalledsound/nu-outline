## React Course Outline week 2

week 3 old stuff:
object destructuring is in week 1
LIFTING STATE UP important. need a good example maybe do image liking in this week?
(but abramov and others now not so interested in it)

#

i'd like to add importing images

### week 2 : Hooks, State, Router

## let's flip the old order and start with Router??

#### v1 what is a SPA ( 3-5 mins)

#### v2 react-router (3-5 mins)

#### v2 react-router in our project (7.5 mins)

    -- Router in index
    -- Switch, Route, Redirect in App
    -- let's make some page stubs for Contact, About and

#### v3 Header (10 mins?)

    -- link vs Link

#### v4 Footer (5 mins)

#### v5 Subheader (Breadcrumbs) (5 mins)

#### v6 make our homempage

    -- HomePage with Menu component and MenuCard

#### v7 moar pages

    -- download AboutPage, ContactPage
    -- CampsiteDirectory Page
    -- NOW what we need is a way to select a campsite

#### v8 10 mins HOOKS overview + comparison to class-based components

    -- What is a 'hook'?
    -- what are the main hooks?
        useState
        useEffect
        -- should I mention these or others that we won't be using?
        useRef
        useCallback
        useMemo
        useReducer
        useContext

    -- why were they introduced?
    -- are there alternatives?  not really but in some old code you will see class based components like this example here
    -- generally hooks replace the most important elements of class based components
    -- one reason they're better is, they are specific to a certain task
    -- this is good functional programming!!!
        -- hooks can't be called conditionally.
        also this stuff we can't do with hooks, nice summary:
    https://owenconti.com/posts/hooks-can-only-be-called-inside-the-body-of-a-function-component-reactjs-error

#### v9 useState

    --useState()
    -- lets access 'state'
     -- [enclosedValue, functionToUpdate ] = useState(initialValue)
    -- (array destructuring aleady covered but remind them)
    -- should we cover closures/how useState actually works?

#### v10 make a clickable heart with FA

    --clickable heart with FA
        -- ternary operator

#### v11 useState on CampsiteDirectoryPage

    -- lifting state

    -- Selected Campsite
    -- useState on Campsite Directory Page for selectedCampsite -- >
    -- campsiteDetail component on same page

### v12 and finally : params + useParams()

--CampsiteDetailPage
-- move campsite detail to a new page and use the cool hook

### should this be extra? or included at all?

### v15 OPTIONAL understanding useState by building it

    -- module pattern and closures in javascript

# week2 workshop:

TOPICS FOR REVIEW:
similar to week 3 workshop.
new Feature: partners
-- PartnersList
-- Partner
-- get data from shared
AboutPage

extras
https://www.youtube.com/watch?v=TNhaISOUy6Q
