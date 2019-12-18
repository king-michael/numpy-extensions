# numpy-extensions
Numpy Extensions


# Functions

## fast_implementations
Implementation of faster algorithms for some numpy core functions by limiting them to single cases.
* `np_unique_int(array, return_counts=False)` <br>
    Fast variant of ``np.unique(array, return_counts=True)`` <br>
    Only works with integer values.
     
## big_data
Methods and Classes to handle data which is to big for the memory.
* `MemoryMapList(npy_files)` <br>
    Class to combine multiple MemoryMap files into one without loading them into memory. 
    It allows to memory map multiple files and handle them as one.
* `NumpyDataset(npyfiles, dtype=None, verbose=False)` <br>
    Class that implements a numpy dataset 
    * `get_sample(self, percentage=None, n_samples=None, size=None, replace=False)` <br>
        Get a sample of the dataset. <br>
        Only of the options `['percentage', 'n_samples', 'size']` is usable at one time.
    
## utils
Utility functions
* `sliding_window(data, size, stepsize=1, axis=-1, copy=True)` <br>
     Calculate a sliding window over a signal <br>
     original code from: https://gist.github.com/nils-werner/9d321441006b112a4b116a8387c2280c

* `npy_header_offset(npy_path)` <br>
    Get the byte offset of a npy file.
    
* `npy_header(npy_path)` <br>
    Get the header of a npy file.