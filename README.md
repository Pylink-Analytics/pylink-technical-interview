# pylink-technical-interview

## Getting Started

- Create a new **private** repository under your own account
- Grant admin access to the `douglas-peter` GitHub user
- Create a `.gitignore` file so generated files won't be committed
- Commit your progress frequently and with descriptive commit messages
- All your answers and solutions should go in this repository

## Keep in mind

- You can use any resource online, but **please work individually**
- **Don't just copy-paste** your answers and solutions, use your own words/code
  instead
  
## After you've finished

- Submit the link to your GitHub repository
  
## Task
  
### Farmer's Field

Now you are going to create a simple farm
where you can take care of your animals.

#### Animal

Each Animal has a name, weight and a product. The animals only start to produce
their product when they reach a weight of 3 units.

- The animal has a `status()` method. It should print the status for an animal.

  - For example: `Daisy, weight: 9, product: milk, has spots: true`

- The animal has a `feed()` method. The implementation should depend
  on the type of the animal.

##### Cow

Cow:
- Gains 1 unit weight when fed
- Produces milk
- Can **randomly** have spots.

##### Sheep

Sheep:
- Gains 1 unit weight when fed
- Produces wool

##### Chicken

Chicken:
- Gains 2 unit weight when fed
- Produces eggs

**HINT:** Cows, Sheep and Chickens are all inherently Animals

#### Field

- It has an `add_animal()` method where you can add animals to your field.

- It has a `feed()` method that feeds all the animals in the field:

  - Increases the weight of every animal by the amount of units
    they gain when fed.

- It has a `remove_animal()` a method that automaticall removes old animals: 

  - If an animal's weight is at least 11 units then it is removed.

- The field has a `get_status()` method which should print
  the status for each animal.
  
 #### N.B.
 There should be a calling method which allows someone to interact with their
 field until they choose to stop doing so. (*This can simply be a command line UI*)
