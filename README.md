# BasicCalculus
Simple library to perform basic 1-dimensional calculus operations in real time. It uses an [alpha-beta filter](https://en.wikipedia.org/wiki/Alpha_beta_filter) to smoothen and numerically differentiate a variable. The library can also integrate the variable should one choose to. Note that it relies on polling to provide a continuoustly changing value. Therefore, one must constantly call an update function to refresh the calculus operations.

# Other
For the sake of simplicity, the library uses micros() to update the timestep, and this step is shared by all instances of alpha-beta filter. This reduces memory usage as just a single variable is required.
