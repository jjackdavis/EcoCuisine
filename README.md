# EcoCuisine


## Setup

```bash
npx pnpm install
npx pnpm astro build # might not work for now
npx pnpm astro dev
# runs a local server at localhost:4321, make sure this port isn't blocked
```


## TODO

- Update information on recipe/pantry cards
  - Maybe make pantry cards smaller (see 'The Team' page)
- Update routes for Add Item to Pantry and Generate New Recipes
- Create more hard coded pantry items and recipes

Have a recipes / home page
Pantry page
EcoBlog with community recs (these recipes are popular among your friends)
The team

## Layout

- Landing page
  - Add fake auth, with preferences
  - Have a refresh button to generate new recipes?
  - Demo would start with user already signed in
  - Have hard-coded recipe cards (keeping in mind pantry stuff / user prefs)
- Navbar
  - Profile (dead link)
  - Pantry page
  - Help (dead link)
- Pantry page
  - Use same card-based UI to display pantry items
  - Have an add to pantry / edit pantry button somewhere

- Recipe Card (look for existing components)

| Title |
Picture

- Ingredients
- [ ] Made,
- Prep Time
- EcoChef rec level :
  - sort by priority based on when things expire
- Macros
- Click to view the recipe
- What did you think, rate it out of 5? (Ideally track this info) to tune recs
- Did you like this? then check this out ->

- Pantry item card (reuse recipe card and rename fields)

| Title |
Picture

- Expiration Date
- Quantity
- Nutrition info
- Maybe add categories
  - Produce
  - Meat
  - Dairy
  - etc.
