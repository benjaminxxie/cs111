# A Kernel Seedling
Program that outputs the # of current running processes on machine

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko
cat /proc/count
```
The module is inserted into the kernel by the first command, and the number of processes that are now running is printed to the terminal window by the second.
## Cleaning Up
```shell
TODO: cmd for cleaning the built binary
```

## Testing
```python
python -m unittest
```
TODO: results?

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
TODO: kernel ver?
