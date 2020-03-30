# Evolution:

## Basic idea of evolution:

- Everyone has some familiarity with evolution

1) Creatures that are better at reproducing, reproduce more, so future generations will be better than those around now.

2) Random mutations in the population are often detrimental, but those few mutation that are "good" (i.e. benificial to reproduction) have a chance at spreading in the population.

## Ingredients for evolution:

For evolution to take place you need a population that:

- has variation (population is not uniform)

- undergoes selection (some individuals are more "fit")

- and reproduces with heredity (offspring gain characteristics of parents)

## Evolutionary algorithm:

- In natural evolution the accumulation of benifitional mutations can produce better adapted organisms.

- A genetic algorithm(GA) is an attempt to capture this "evolutionary improvement system"

## The GA:

An evolutionary algorithm simulates a population of individuals that

- Reproduce by hereditability

- are mutated to produce some kind of variability

- are selected through some measure of fitness

## An example situation - Evolving a paper glider:

    1. Generate 20 random sequences of folding instructions.
    2. Fold each piece of paper according to the instructions written on them.
    3. Throw them all out of the window.
    4. Pick up the ones that went furthest, look at the instructons.
    5. Produce 20 new pieces of paper, writing on each bits of sequences from parent pieces of paper.
    6. Repeat from (2) on.

## Human Design vs. Artificial Evolution

- An evolutionary standpoint introduces biases not normally considered in typical human design

- essentially it is blind variation vs human design (which is the breakdown of a system into its componenets)

**Biases**:

- unlike, human design, GAs are not biased towards non-intuative shortcuts for solving problems.

- The biases are not easy to identify but rely on how mutation takes place

One thing to consider is that Gas cannot produyce a solution in one step like human design. Rather, it will produce this over a number of generations.

## GAs influence in disciplines

- Science (helping us to understand natural evolution in more depth)

- Engineering
    - Engineering design in unorthodox methods
    - Scheduling problems
    - Container load optimisation

## GA example - evolving airfoil in a wind tunnel (Disciplinary example - engineering)

Ingo Rechenberg 1964

    1. Change (mutate) a random angle by a small amount (small changes mroe likely)
    2. Measure drag. If it is worse undo the changes.
    3. Go to 1

## Genotype/Phenotype representation

- Genotype (The genetic makeup of a cell)

- Phenotype (One characteristic within a genotype)

## How this is used in our Rechenberg example:

- Genotype: the angle of each aerofoil
    - g0 = [a1, a2, a3, a4, a5, a6, a7, a8]

- Phenotype: The shape of the wing
    - Each aerofoil has this characteristic.

- Fitness: The amount of drag on the wing due to airflow.

## Fitness:

- In the natural world, fitness is determined by many complex interacting factors.
    - e.g. Predator/ prey coevolution, sexual selection, competition with conspecifics( a member of the same species), luck (e.g. meteor strike).

- BUT! evolutionary algorithms are not the same thing. There is often a clearly defined "fitness function" guiding evolution towards a predetermined objective.

## Hill climber psuedo code (barely evolution at all to some people)

    1. Randomise the genotype (g0 = [a1, a2, a3, a4, a5, a6, a7, a8])
    2. Copy Genotype to temporary genotype (g1 <-- g0)
    3. Mutate g1 (Increment the angle of one allele - allele is a variant form of a gene)
    4. Evaluate fitnesses (Measure drag)
    5. if (Fitness(g1) > Fitness(g0))
            g0 <-- g1
        else
            do nothing
        end
    6. Goto 1











