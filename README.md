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
## Debug
modinfo proc_count.ko. - view module info
sudo dmesg -l info - view logs
sudo rmmod proc_count - stop running the kernel module
## Cleaning Up
```shell
make clean
```
This will clean up all files created in the build process.
## Testing
```python
python -m unittest
```
Passes all 3 tests on Arch Linux 5.14.8. To get the kernel version, run the following command:

```shell
uname -r -s -v
```
