# Exponential Moving Average
This algorithm applies an [explonential moving average](https://en.wikipedia.org/wiki/Exponential_smoothing) to the raw results of an observed algorithm execution and then compares the result to a threshold. If the result is **below** the threshold the algorithm signals the presence of dataset shift (returns 1).

## Parameters
- **alpha**: weight that multiplies the most recent sample (also check out the wikipedia article in the link above). Must be in (0,1).
- **threshold**: the number to be compared with the result of the exponential moving average applied to the input.

## Limitations
The raw results of the observed algorithm execution must be parsable as floats.