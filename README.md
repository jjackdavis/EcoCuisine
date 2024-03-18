# EcoCuisine

## TODO: 
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



## FAQ

<br/>

<details>
  <summary>What is this?</summary>
<br/>
  This is a astro template that uses tailwindcss and alpinejs
</details>
<br/>

<details>
  <summary>Why alpinejs? Why don't just use js?</summary>
<br/>
  Alpine js is less than 17kb and it make javascript very fast to write, there are also various open source ready to use components like https://js.hyperui.dev, https://devdojo.com/pines, https://www.alpinetoolbox.com/examples, https://alpinejs.dev/components#components
</details>
<br/>

<details>
  <summary>But I don't need alpine js, can I remove it?</summary>
<br/>
  Of course, but some components use it and you'll have to edit these, more specifically you ll have to: <br/>
  <ul style="list-style: inside;">
    <li>First remove the package with the command <code>npm unistall @astrojs/alpinejs @types/alpinejs alpinejs</code></li>
    <li>Adjust all components that uses alpine js: <code>faq.astro</code>, <code>themeselector.astro</code>, <code>navbar.astro</code></li>
  </ul>
</details>
<br/>

<details>
  <summary>Can I remove also tailwidcss?</summary>
<br/>
  I mean, you can, but you'll have to basically rewrite all the template, so I don't recommend it
</details>
<br/>

<details>
  <summary>I don't need client routing, how can I remove it?</summary>
<br/>
  From astro 2.9 you can opt-in for client routing (https://astro.build/blog/astro-290) by activating the experimental flag viewTransitions <br/>
  You can remove client routing by removing <code>viewTransitions: true</code> from <code>astro.config.mjs</code> And the <code>ViewTransitions</code> component from Layout.astro
</details>
<br/>

<details>
  <summary>I don't need multiple language, how can I remove it?</summary>
<br/>
  One way is to simply keep one language and remove the selector from the footer but in order to fully remove the localization you have to: <br/>
  <ul style="list-style: inside;">
    <li>Remove the i18next pacakage <code>npm unistall astro-i18next</code></li>
    <li>Remove <code>astro-i18next.config.mjs</code> file</li>
    <li>Remove <code>locales</code> folder from public</li>
    <li>Remove <code>languageselector.astro</code> file and from footer</li>
    <li>Find all reference to <code>i18next</code> and <code>astro-i18next</code> and replace with your text</li>
  </ul>
</details>
<br/>

<details>
  <summary>I don't need dark mode, how can I remove it?</summary>
<br/>
  Dark mode is embedded into tailwindcss, so you can't remove it, but you can remove the switch from the navbar
</details>
<br/>


<details>
  <summary>How can I configure the Sveltia CMS authentication with cloudflare?</summary>
<br/>
  To configure Sveltia CMS with cloudflare follow this guide <a href="https://github.com/sveltia/sveltia-cms" target="_blank">https://github.com/sveltia/sveltia-cms</a>
</details>
<br/>


<details>
  <summary>How can I change the localization languages?</summary>
<br/>
  In order to change the languages you have to change the languages in the file <code>astro-i18next.config.mjs</code> and in the netlifyCMS configuration on the file <code>astro.config.mjs</code> <br/>
  Then change the locales files folders in <code>public/locales</code>
</details>
<br/>

<details>
  <summary>What are the files in the function folder used for?</summary>
<br/>
  These are cloudflare function that are used for the authentication to the decap CMS
</details>
<br/>

<details>
  <summary>The build on cloudflare keep failing, why?</summary>
<br/>
  One of the problem could be that the Build system version is setted to version 1, make sure that version 2 is selected
</details>
<br/>

<details>
  <summary>Work with modules in relink</summary>
<br/>
  This is helpful if you want to apply some changes to various modules while you are working on the website.
To do so you have to go into each module and run

```
npm link
```
</details>
<br/>

---

<p align="right"><a href="https://zank.studio/" target="_blank">zank.studio</p>
