# Pokedex-ROR
Pokedex app built with Ruby on Rails. This project started as a learning exercise and evolved as I become more knowledgeable in various technologies.

The site can be viewed [here]().
Initial load may take a while as it is hosted on Heroku.

This Rails project served as a sandbox for me to practice and learn the fundamentals of web development. As a result, the current codebase is full of comments and WET code.

I'm currently in the process of rewriting the codebase for this project.

---
The project started as a means to learn the fundamentals of ActiveRecord and database relationships. I fetched data from the [PokèAPI](), created various models, and in `seeds.rb` persisted the data into the database with ActiveRecord methods.

![](/Schema.png)

As I became more committed to learning web development, I revisited this project and built upon it by adding addtional features and applying the things I learnt.

![](/Screenshot1.png)
![](/Screenshot2.png)
![](/Screenshot3.png)
![](/Screenshot4.png)

## Built With
- [Rails 6](https://guides.rubyonrails.org/) - Backend / Front-end
- [Stimulus JS](https://stimulus.hotwired.dev/) - Front-end JS
- [Bootstrap](https://getbootstrap.com/) - Front-end - popover / tooltips
- [Heroku](https://heroku.com/) - Deployment

## Todo

### Rewrite
General
 - [ ] Rewrite HTML to minimize reliance on bootstrap
 - [ ] Use Semantic HTML
 - [ ] Rewrite CSS following the BEM methodology
 - [ ] Make use of CSS variables. Create a design system instead of using random values for spacing, font-size, etc.

 - [ ] Routes

 Seed File
 - [ ] Refactor WET code
 - [ ] Documentation for seed file

Index page
  - [x] Refactor ActiveRecord queries in the model for search
    -  [x] Create scopes
    -  [x] extract search to class method
  - [x] Move 'clear filter' button to take up own line on mobile
  - [x] Eliminate n+1 queries
  - [x] Create rails helper for 'no_results'

Show page
  - [ ] Think in terms of components - Create components and build page with them
  - [ ] Extract navigation to custom rails helper method
  - [ ] Figure out how to eliminate n+1 queries

### Models
  -
### Controllers
  -
### Partials
  -

### Bugs
  - [x] Button to toggle normal and shiny images - make fixed width
  - [x] Slow Ajax/ index page load. -- figure out how I can speed it up
  - [ ] Reset filters when clicking randomize
  - [ ] Make the Shiny/Normal button fixed width
  - [ ] Firefox Select bug - https://stackoverflow.com/questions/16615346/problems-with-html-select-firefox / https://stackoverflow.com/questions/71213370/select-element-in-firefox-wont-stay-open-when-parent-div-has-a-pseudoelement-on

### Additional pages/features
Important
  - Eeveelutions missing evolution chain component on show page - need to code a custom component for it
  - Add Error Page - https://www.pokemon.com/us/pokedex/evolutions/

Not important
  - Link that links to a random pokemon show page
  - Type Page - e.g lists all fire pokemon - shows the count of pokemon with that type -'There are xx Grass Pokemon in Gen1 + Gen 2'
  - Ability Page
  - Egg group page
  - Section showing specific Strong/Weak/Immune against Pokèmon
  - Unown - Shiny images not uploaded
    - Create an image section showing all Unowns

### Old
<del>
General
  - [x] More noticeable indication when hovering over pkm  - pokemon.com/uk/pokedex
  - [x] 'Suprise me!' function - returns a subset of results - pokemon.com/uk/pokedex
  - [x] Fix Type sorting - Add a new attribute to PokemonType model that holds the slot number - That way I can remove the sort type method and just order by slot number
  - [x] Fix Ordering of the Pokedex hash

Search
  - [x] Create a search function that displays the full list of pokemon and filters them out based on the input in the search field
  - [x] Update search functoion so it can search for for a Pokèmon by name or using its National Pokèdex number
  - [x] Re-implement search with StimulusJS
  - [x] Redo search to use AJAX. (previously done via loading all the data and toggling the css rule `display: hide`)
  - [x] Figure out how to debounce search
  - [x] Create a second search in the nav bar that becomes active when the main search bar is not in view
  - [x] Figure out how to link the second search bar to the main search bar controller

  - [x]  Add randomize button that randomizes the list of Pokemon

  - [x] Filter by Type
  - [x] Sort results by
    - [x] lowest number (first)
    - [x] highest number (first)
    - [x] A-Z
    - [x] Z-A
    </del>
