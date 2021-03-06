# Cybernetic Optimization for Complex Systems

Generally, complex systems are artificially stabilized and optimized in the same way that linear systems are. Sometimes, higher-order components are accounted for by differentating or integrating but, overall, feedback systems are designed such as to minimize deviation from local optima at all times.

When comparing this to most naturally evolved sytems, however, we can see that they are often grown to gain from disorder; rather than requiring or assuming an environment that is consistant, they thrive and grow from unexpected perturbations. In another way, it can be said that these 'anti-fragile' systems learn.

As an increasing amount of societies processes have effectively been cybernetically regulated in one way or another, it should become increasingly apparent that this 'overfitting' has become a systemic weakness as large perturbations occur with increasingly dramatic disruptions as a consequence.

Alternatively, it shoud be possible to design control loops such as to account, specifically, the non-linearities in the dynamics by careful fuzzing of the control system. This implies the conscious injection of noise in the control signal in order to determine the degree of fragility of systems, to discover couplings between components and to explore and model the full operating space of the system rather expecting it to be calibrated to a particular local minimum. This mimicks, much closer, the operation of natural cognitive self-learning systems such as ourselves.

Of course, care should be taken here to only explore the safe operating space of systems, and in a sense this different type of control structure should be embedded in the very design of systems; in case of failure of the operating circuit of the sytem, it should degrade gracefully to a basic 'unoptimized' way of functioning or temporarily stop to operate. In a sense, it implies that systems should, essentially, be design to fail.

The idea, furthermore, is to design systems such that they are self-optimizing under continuously and qualitatively changing conditions. There could be a collection of algorithms such that, given any amount of inputs and outputs and given certain, potentially dynamic, optimization conditions, the system learns itself how to optimize. 

Typically, such a problem solving system would be fed any known relations or other assumptions about the system (i.e. units of measurement, ranges of inputs and outputs) and a safe domain for fuzzing of the control parameters. Based on this it would create a collection of models based on past behaviour of the system but accounting for hidden interactions and changes in circumstances. 

These models, together with the given optimization conditions would result in problem sets, the solutions to which encompass optimization strategies. These strategies will be weighed, based on fitting performance of the model, optimization performance and fragility (ability to deal with unexpected perturbations) and based on the weight a different strategy might be chosen at any time.

However, the system continually refines its strategies and models using genetic algorithms together with random perturbations of control strategies and models. Essentially, this means that the system continually 'guesses' models (typically based on a given Ansatz) and then further refines them by combining them with others, all the while combining until sufficient solutions are found.

### Further notes
* Account for path-dependence in model creation
* Clear distinction between inputs (only natural 'noise') and outputs (fuzzable)
* Account for interactions between inputs/outputs, specifically perturbations
* Test for and, then, assume local continuity within current local optima
* Dynamically map paths amongst local optima, creating self-optimizing systems