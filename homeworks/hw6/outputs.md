# Výsledky
## 1. Model: <ins>unsloth/Llama-3.2-3B-bnb-4bit</ins>
---
### Prompt:

Create a magical recipe for an 'Elixir of Clarity'.\n\n**Ingredients:**\n* 1 drop of morning dew from a forgotten forest\n* 3 petals from a moonflower\n* 1 pinch of stardust\n\n**Preparation Steps:**\n1. Collect dew at dawn.\n2. Gently press moonflower petals into a vial.\n3. Add stardust to activate.\n\nNow, create a magical recipe for an 'Elixir of Dreams'. List the mystical ingredients needed and the detailed preparation steps to brew it.

### Output:

Mystical Ingredients and Preparation Steps for the 'Elixir of Dreams':

**Ingredients:**
1. A piece of the moon's white cloak
2. A crystal ball of star dust
3. A golden vial with a cap
4. A bottle of black oil

**Preparation Steps:**
1. Gather the ingredients.
2. Wash the cloak and remove any dirt.
3. Place the cloak on the crystal ball.
4. Pour the black oil onto the crystal ball and mix.
5. Add the gold cap to the bottle.
6. Shake the bottle vigorously until a seal appears.
7. Store the vial in a safe place.

Remember, the elixir must be crafted with great care and respect for the nature spirits and elements to be truly powerful and beneficial.

### Output:

**Elixir of Clarity Recipe**
>1 drop of morning dew from a forgotten forest
>3 petals from a moonflower
>1 pinch of stardust

**Preparation Steps**
1. Collect dew at dawn.
2. Gently press moonflower petals into a vial.
3. Add stardust to activate.

**Ingredients for Elixir of Dreams Recipe**
* 1 moonstone
* 1 piece of dark velvet
* 1 bottle of clear essence
* 1 bottle of sweet essence
* 1 piece of lavender

**Preparation Steps**
1. Place moonstone and dark velvet in a small container.
2. Pour clear and sweet essence into a cauldron.
3. Light the lavender and allow to smolder for a few moments.
4. Pour the essence into the cauldron and stir until well combined.
5. Place the moonstone and dark velvet into a clear vial and seal tightly.

### Output s rovnakým promptom, no nedotrénovaným "originálnym" modelom:

1. A mixture of 2 tablespoons of olive oil and 3 tablespoons of honey in a container with a tight lid.
2. Place the container in the fridge and refrigerate overnight.
3. Take out the mixture and place the container on the stove at medium temperature (not too hot, nor too cold). While gently stirring the mixture with a wooden spoon.
4. Once the mixture has started to boil, add one spoonful of hot water, stirring as you add it.
5. Repeat step #4 three times.
6. When done, take out the mixture, cover with a cloth, and let the mixture rest in the refrigerator overnight.

`%Explain the process`
`%What do each of these mean to us?`
`%The purpose of each ingredient`
`%Their effects`

**What are the advantages to knowing all this?**
* Better understanding of how each step works

`%How to improve a recipe?`

**When you've created your 'Elixir of Clarity', let's test it out!**




---
## Rovnaký model, no menší počet epoch a kratší prompt:
Create a magical recipe for an 'Elixir of Dreams'. List the mystical ingredients needed and the detailed preparation steps to brew it.

### Output:

In this tutorial, we will learn how to create and run a simple Elixir application using the Ecto framework and SQLite.

I. Prerequisites

Elixir 2.5, Erlang 23, and Redis

II. Application and Database Configuration

To create and run our application, we must first create a new directory, `magical_recipe` and initialize our project using `mix`:

`cd /path/to/magical_recipe`
`mix new magical_recipe`

This will create the necessary directory structure for our application and generate an initial `mix` executable.

We can then set up a local development SQLite database and seed our tables with some initial data. For this, we need to create a new file called `config.exs` and add some configuration for our SQLite database and Ecto migrations.

In our new `config.exs` file, we will set up the SQLite database using `use Mix.Config`, and configure the database adapter and URL, and seed our `magical_recipes` table with the following recipes:


---

## 2. Model: <ins>unsloth/Llama-3.2-3B-Instruct-bnb-4bit</ins>
Model stavaný na odpovedanie na inštrukcie usera.

### Prompt:
Create a magical recipe for an 'Elixir of Clarity'.
### Output:
**The Elixir of Clarity: A Magical Recipe**

In the realm of mysticism, the Elixir of Clarity is a rare and precious potion said to grant the drinker clarity of mind, focus, and mental agility. This enchanted brew requires precision, patience, and a deep understanding of the universe's harmony.

**Ingredients:**

1. **Luminous Petal of Clarity**: A rare, delicate flower that blooms only under the light of a full moon. Its petals are said to hold the essence of clarity and focus.
2. **Golden Ambrosia**: A fragment of the golden nectar collected from the ambrosial tree of ancient wisdom. This sacred ambrosia amplifies the elixir's effects.
3. **Mindstone Essence**: A crystalline extract from the heart of the Mindstone, a mystical mountain said to harbor the secrets of the universe. This essence enhances cognitive functions and mental clarity.
4. **Stardust Dusting Powder**: A pinch of stardust collected from a shooting star's trail. This magical powder imbues the elixir with cosmic energy and mental sharpness.
5. **Ethereal Lavender Oil**: A vial of lavender oil infused with the essence of moonflowers. This


### Output s rovnakým promptom, no nedotrénovaným "originálnym" modelom:

**Elixir of Clarity Recipe**

In a realm where magic and mystery entwine, we present to you a recipe for the enchanted Elixir of Clarity. This mystical drink is said to grant clarity of mind, sharpness of thought, and insight into the unknown.

**Ingredients:**

1. **Moonpetal Blooms**: Rare and exquisite, these delicate flowers bloom only once a year, under the light of a full moon. Harvest the petals at dawn, when the dew is still fresh.
2. **Starlight Salt**: A pinch of salt harvested from a celestial spring, imbued with the essence of stardust and the whispers of the cosmos.
3. **Dreamweaver's Honey**: A drizzle of pure, golden nectar collected from the hives of rare, moon-pollinated bees.
4. **Crisp Clearwater**: Freshwater collected from a crystal-clear lake, filtered through the leaves of the Luminous Fern.
5. **Essence of Luminous Moss**: A subtle, shimmering extract obtained from the delicate, glowing threads of the Luminous Moss that grows on ancient, mystical trees.

---
## Rovnaký model, no vyšší počet epoch:
(output basically the same)


**The Ancient Recipe for the Elixir of Clarity**

In the mystical realm of Aethoria, where the sun dipped into the horizon and painted the sky with hues of sapphire and amethyst, the wise sorceress, Lyra, revealed to us the secrets of the Elixir of Clarity. This enchanted potion is said to grant the drinker unparalleled mental acuity, clarity of thought, and unwavering focus.

**Ingredients:**

1. **Moonpetal Blooms**: Rare, delicate flowers that bloom only under the light of the full moon. Their petals hold the essence of lunar magic, which amplifies the drinker's intuition and psychic abilities.
2. **Starlight Dust**: A pinch of stardust collected from the heart of a shooting star. This celestial ingredient imbues the elixir with the power of celestial guidance and wisdom.
3. **Essence of Clarity**: A vial of pure, crystalline water distilled from the crystal caves of the ancient mountains. This essence clarifies the mind, allowing the drinker to see through deception and illusions.
4. **Golden Ambrosia**: A drizzle of golden honey harvested from the hives of sacred bees. This ambrosial nectar enhances cognitive function,

