
## What is needed?
|            |Time limit   | Cutoff  | Advance   |
|---         |---          |---      |---|
|Speed events| x  | x   | x  |
|FMC         | -  | x  | x  |
|MultiBLD    | -  | x  | x  |


The time limit for FMC and MultiBLD is always 1h.

## Units
The general approach how time limits, cutoffs and advance conditions are handled is the same for all types of events.
The (important) difference are the units how the results are measured:

* Speed events: time 
* MultiBLD: points
* FMC: moves

## Some restriscitons and conditions
### Time Limits
* Default is 10 minutes for speed events

### Cutoffs
* Number of attempts for "full" round format `>` attempts for first phase of combined round
    * e.g setting the format of the round to "Best of 3" and the format of the combined round to "Average of 5" is not possible
* The cutoff time must not be higher than the time limit.

### Advance conditions
* Percentile `<=` 75%
* Advance condition `<` Time Limit


## Some design ideas
### Time limit

#### Individual Time limit
Set the time limit for an individual attempts (default selection):

![](images/time-limit-individual.png)

#### Cumulative Time limit
Set a cumulative time limit. To clarify that this is a cumulative time limit for a single round, the name of the round is shown below.

![](images/time-limit-cumulative-1.png)


To add an additional round (and make this a cumulative time limit for 2 events), click on "Add round":

![](images/time-limit-cumulative-2.png)


### Cutoff
#### Set Cutoff
The default selection is "None", which means that no cutoff was set for the round:
![](images/cutoff1.png)

#### Choose a format
To change this, the format of the combined round has to be chosen. The right side represents the format that was chosen for the round:
![](images/cutoff-choose-format.png)

#### Add the cutoff time
Selecting a round format for a combined round reveals another row where the cutoff can be added:
![](images/cutoff-add-result.png)

### Advance conditions
Three types to choose from:
![](images/advance.png)
