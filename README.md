# StarWars
React-Redux Application with Swapi

# Dependencies

Node / NPM - Tested with Node v8.11.0.

*Some interesting dev dependencies to be used:*

Autoprefixer: Write your CSS rules without vendor prefixes (in fact, forget about them entirely)

# Get Started

`npm install` - to install project dependencies.

`npm run dev` - to start webpack dev server and watch for changes.

`npm run build` - to create production ready build.

`npm run test` - to run test cases.

`npm run lint` - to run code quality tests.

Opens app in new browser window at `http://localhost:7070/`

# Targets

This react-redux application that has two pages targets to achieve the following:

1. Page 1: Login Page

   Allows the user to login as a character from STAR WARS using the

   - character name as the username

   - **birth year as the password.**

   *eg: Luke Skywalker / 19BBY*


2. Page 2: Search Page

   Implements **a type-along search** which searches **for planets** and lists them in components that are sized relative to their diameter on every keypress in the input field.

   **Planet Case Handling**
   Diameter scaling is as:
        dia = (planet.diameter) / 80

   Few planets had really big diameter, so for them Diameter max diameter is limited as:
        (dia) > 300) ? 300 : dia);

   Few planets had 0 diameter they are shown in autocomplete dropdown but you can't choose.

   Only the user Luke Skywalker is enabled to make **more than 15 searches in a minute**.

   Other users can't make more than 15 search in 1 minute

   Other Users after one minute can re search.


Final Check Box:

:point_right: Charting library to create planets

:point_right: a type along search :white_check_mark:

:point_right: Validations in the login page :white_check_mark:

:point_right: Production ready build :white_check_mark:

:point_right: AirBnB ESLint rule beautified :white_check_mark:

:point_right: this.setState() :negative_squared_cross_mark: wherever possible

:point_right: Minimum characters for search is 1 :white_check_mark:

:point_right: User given some time to type before starting a search or in case he/she decide to remove some characters
              as he/she types. :white_check_mark:

:point_right: own **autocomplete component** :white_check_mark:

:point_right: appropriate message in case there is no result. :white_check_mark:

:point_right: separate concerns for both React and Redux. :white_check_mark:

:point_right: Browser hard refresh for new style changes to reflect, not required after every deployment. :white_check_mark:
