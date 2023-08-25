# Kismet: Network Sniffer

Kismet is a versatile sniffer, WIDS (Wireless Intrusion Detection System), and wardriving tool designed for Wi-Fi, Bluetooth, Zigbee, RF, and more. It's compatible with Linux and macOS.

## About the Project

Explore the world of wireless insights with Kismet! This open-source tool offers powerful features:

- Passive capture and monitoring of wireless data
- Wi-Fi, Bluetooth, BTLE, Zigbee, and more protocol support
- Graphical representation of frequency distribution, signal strength, and more
- Device tracking, alerts, and intrusion event detection

## Features

- **Passive Capture**: Kismet works seamlessly in the background, collecting wireless data without user intervention.

- **Wireless vs Wired Monitoring**: Understand the challenges of capturing wireless packets due to various factors, including physical characteristics and driver support.

- **Smart Channel Hopping**: Kismet optimizes channel hopping for comprehensive coverage using strategic scrambling and offsetting techniques.

- **Installation**: Follow the installation guide on Kali Linux using Git repository cloning and package installation.

- **Monitor Mode Setup**: Learn how to put your wireless card into monitor mode for efficient packet capturing.

- **Launching Kismet**: Start Kismet as a non-root user and begin packet capture.

- **Device Information**: Gain insights into tracked devices with details like MAC address, manufacturer, signal strength, and more.

- **Graphical Representation**: Visualize data with historical graphs showcasing Wi-Fi vs clients, frequency distribution, and devices per channel.

- **Persistent Surveillance**: Set up permanent monitoring on specific channels for in-depth network analysis.

- **Security Measures**: Learn how to protect your network by adjusting Wi-Fi power settings and avoiding unnecessary signal broadcasting.

- **Hiding Devices**: Prevent devices from being listed by turning off Wi-Fi when not in use and considering MAC address randomization.

## How to Use

1. **Install Kismet**: Clone the Git repository and install required dependencies on Kali Linux.
   
   ```shell
   git clone https://www.kismetwireless.net/git/kismet.git
   sudo apt-get install build-essential git libmicrohttpd-dev zlib1g-dev libnl-3-dev libnl-genl-3-dev libcap-dev libpcap-dev libncurses5-dev libnm-dev libdw-dev libsqlite3-dev
   cd kismet
   ./configure
   make
   sudo make suidinstall
   ```
2. **Put Your Wireless Card in Monitor Mode**: Use the airmon-ng command to enable monitor mode for your wireless card.

```shell

sudo airmon-ng start YourCardName
```

3. **Launch Kismet**: Start Kismet by specifying the monitor mode card.

```shell

    kismet -c YourCardNameMon
```

4. **Explore and Analyze**: Navigate the Kismet interface, analyze data, visualize graphs, and monitor wireless activity.

## Contributed By

[Vaibhav Mishra](https://vaibhav-mishra.vercel.app/)

Feel free to contribute and enhance the project!

## License
This project is licensed under the MIT License - see the LICENSE file for details.
