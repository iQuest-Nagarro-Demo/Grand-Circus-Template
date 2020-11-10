# Branching

There are two branches in the repository:
- **master** - contains the exercise
- **solution** - contains the solution to the exercise.

## Rules
- Every change in the master branch must be merged in the solution branch.
- Never merge the solution branch back into master.

# Grand Circus - Exercise

## Circus

Create a Console Application that will have a `Circus` class.

The `Circus` needs to receive from outside an `Arena` instance (see the provided code), but it manages internally a collection of animals (creates and keeps a collection with all of them).

## Animals
As any respectful circus, it must have a collection of animals that must implement the `IAnimal` interface.
All the animals are born in captivity, in the Circus, and each animal receives a Name at birth, that cannot be changed.

> Hints
>	- Find a way to ensure that the name of the animal will not be changed after the object is created?

Each animal belongs to a species. This property is not configurable from outside and cannot be changed. It is the nature of each animal. It is, however, visible. It must be easy to obtain this information from each animal.

> Hints
> -	Find a way to avoid duplicating the implementation of the Name and SpeciesName properties in each class.
> -	Find a way to ensure that the Name and SpeciesName are provided for each animal.

## Performance

Having said this, the Circus can now Perform. The performance consists in bringing every animal, one by one, to the arena, announce them and provoke them to make a sound. I know, it is kind of a lousy Circus, but this is all it is necessary to receive prize in the beginning of the world of learning… Remote Learning, I mean.

The classes (Hint):
- `Arena` - It is responsible to display the messages in the console.
- `Circus` - It is responsible to manage the collection of animals.
- `IAnimal` - Represents an animal. It is the abstracted idea of an animal.
- `AnimalBase` - Contains common functionality for all the animals.
- Some animals: 
  - `Elephant` - A concrete implementation of an animal.
  - `Lion` - Another concrete implementation of an animal.
  - `Snake` - Yet another concrete implementation of an animal.
  - Be creative with more animals :)