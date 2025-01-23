# Rust on Raspberry Pi Pico W

After dedicated [a repo to ESP32](https://github.com/m1ckc3b/rust-on-esp32) it's the Pico W turn. I reproduced the same projects that on the ESP still by using the Lafvin Basic Starter Kit components.

With Pico I wanted to only use asynchrone programming so I implemented each project (expect project_0) with the Embassy crate. So that means only on no_std mode.

Few words on the Pico W. Its heart is a dual-core 32-bit ARM Cortex-M0+ (it would cool to use it in multithreading) and it has a wifi module (great for iot projects).

I used this template with `cargo generate` to create each project (expect project_0)

```
$ cargo generate 9names/embassy-rp-quickstart
```

## Projects
- [Project_0](./project_0/) - Blinky
- [Project_1](./project_1/) - Blinky with pushbutton
- Project_2 - Analog Inputs (ADC)
- Project_3 - PWM Analog Output
- Project_4 - PIR Motion Sensor
- Project_5 - Switch Web Server
- Project_6 - RGB LED Web Server
- Project_7 - Relay Web Server
- Project_8 - Output State Synchronization Web Server
- Project_9 - DHT11 Web Server
- Project_10 - OLED Display