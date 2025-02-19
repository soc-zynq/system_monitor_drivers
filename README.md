# system_monitor_drivers

## Description
A simple kernel module with a user-space application.

## Project Structure
```
system_monitor_drivers/
├── kernel_module/
│   ├── src/
│   │   └── system_monitor_drivers.c
│   ├── include/
│   │   └── system_monitor_drivers.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd system_monitor_drivers/kernel_module
make
```

### Application
```bash
cd system_monitor_drivers/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod system_monitor_drivers/kernel_module/system_monitor_drivers.ko
# Do something with the module
sudo rmmod system_monitor_drivers
```

### Application
```bash
cd system_monitor_drivers/application
./test_app
```

## License
GPL
