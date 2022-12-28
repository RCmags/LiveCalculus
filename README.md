# BasicCalculus
Simple library to _approximate 1-dimensional calculus operations_ in real time. It uses an [alpha-beta filter](https://en.wikipedia.org/wiki/Alpha_beta_filter) to __smoothen__ and numerically __differentiate__ a variable. The library can also __integrate__ the variable should one choose to. Note that it relies on polling to provide a continuoustly changing value. Therefore, one must constantly call an update function to refresh the calculus operations.

# Other
For the sake of simplicity and to reduce memory use, the library uses micros() to update the timestep, and this step is shared by all instances of alpha-beta filter.

