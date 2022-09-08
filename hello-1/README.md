# Overview
This code represents the simplest kernel module you can create

# Key concepts
 - A kernel is the primary interface between the hardware and the processes of a computer
 - We can add our own code to the kernal by writing specialized C code
 - A kernel module has a method to initialize the module and reserve resources
 - A kernel module also has a method to clean up resources reserved during initialization
 - Make files build code into binaries the computer can execute
 - Make files use tabs for indentation

# Commands

## Building the code
- Change to the hello-1 directory
```
cd <project root>/hello-1
```
- Build the code
```
make
```

## Load the module
- The insmod tool is used to load kernel modules
```
sudo insmod hello-1.ko
```

## Check that the module is running
- The lsmod tool lists modules
- The grep tool filters text based on a pattern
```
sudo lsmod | grep hello
```

## Remove the module
- The rmmod tool removes modules
```
sudo rmmod hello_1
```

## View kernel logs
- the journalctl tool lets you view kernel logs
```
sudo journalctl --since "1 hour ago" | grep kernel
```

# Comprehension questions
- How can you list all kernel modules?
- How can you filter for a different kernel module?
- Can you change the messages printed to the kernel logs?

# Further reading
- https://sysprog21.github.io/lkmpg/#hello-world