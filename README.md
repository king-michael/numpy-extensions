# numpy-extensions
Numpy Extensions


# Functions

## fast_implementations
* `np_unique_int(array, return_counts=False)` <br>
    Fast variant of ``np.unique(array, return_counts=True)`` <br>
    Only works with integer values.
    
## utils
* `sliding_window(data, size, stepsize=1, axis=-1, copy=True)` <br>
     Calculate a sliding window over a signal <br>
     original code from: https://gist.github.com/nils-werner/9d321441006b112a4b116a8387c2280c
