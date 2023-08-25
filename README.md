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

  ![devices](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/5d9a2aad-188f-4b3b-8706-5ec1903016a3)


- **Wireless vs Wired Monitoring**: Understand the challenges of capturing wireless packets due to various factors, including physical characteristics and driver support.

- **Smart Channel Hopping**: Kismet optimizes channel hopping for comprehensive coverage using strategic scrambling and offsetting techniques.

- **Installation**: Follow the installation guide on Kali Linux using Git repository cloning and package installation.

- **Monitor Mode Setup**: Learn how to put your wireless card into monitor mode for efficient packet capturing.

- **Launching Kismet**: Start Kismet as a non-root user and begin packet capture.

- **Device Information**: Gain insights into tracked devices with details like MAC address, manufacturer, signal strength, and more.

  ![Screenshot_46](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/a622e15a-509c-45f8-8d53-e882bd041004)

  ![Screenshot_42](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/f8a2dcd1-9117-4d63-8037-b5307ee1cb4b)


- **Graphical Representation**: Visualize data with historical graphs showcasing Wi-Fi vs clients, frequency distribution, and devices per channel.

  ![Screenshot_2022-11-14_01_35_48](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/5f9c46cd-b46f-410b-92af-ab1b4a1c3458)
  
  ![Screenshot_2022-11-14_01_36_04](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/1c578d99-d328-4fb3-88e4-34df0af55f88)


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
   
   ![Screenshot_42](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/b47a4032-6c04-4f52-9e85-7124015fee3a)


4. **Explore and Analyze**: Navigate the Kismet interface, analyze data, visualize graphs, and monitor wireless activity.
   

  ![Screenshot_2022-11-14_01_39_45](https://github.com/VaibhavMishra1341/Kismet/assets/39896268/503aebb4-d7ab-48c9-a435-9c4133333eb3)

## Contributed By

[Vaibhav Mishra](https://vaibhav-mishra.vercel.app/)

Feel free to contribute and enhance the project!

## License
This project is licensed under the MIT License - see the LICENSE file for details.
