# LAMP-Stack-Task

## Task 1

Steps - 

1. Downloaded VMware to run the iso file of the OS.
2. Instead of removing the GUI completely, I just set up the **grub** to stop the **GUI** from loading on boot and instead give us the text login, so that I could restore it later if required.

    Command -
    ```
    systemctl set-default multi-user.target
    ```
    
3. Then we get ```Command Line Interface (CLI)``` on rebooting.


**A hacky solution** - We can also download the iso of minimal CentOS-7 directly. It contains only the CLI and no GUI.

## Task 2

### **The OSI Model**

The ```OSI (Open Systems Interconnection)``` model is a conceptual framework for understanding how communication between different computer systems and devices takes place. It consists of seven layers, each of which has a specific set of functions and protocols that work together to facilitate communication.

Here is a brief description of each of the layers of the OSI model, starting from the lowest layer:

1. **Physical Layer**: The physical layer deals with the physical transmission of data over the network. It specifies the physical characteristics of the transmission medium, such as the voltage, current, and signal rate. It also defines the connector types and cable specifications.
2. **Data Link Layer**: The data link layer is responsible for transferring data between two nodes on the same network. It ensures that data is transmitted without errors and provides a mechanism for detecting and correcting errors.
3. **Network Layer**: The network layer is responsible for routing data between different networks. It decides the path that data takes through the network and handles addressing and packet fragmentation.
4. **Transport Layer**: The transport layer provides end-to-end communication between two devices. It ensures that data is delivered reliably and in the correct order.
5. **Session Layer**: The session layer manages the connection between two devices. It sets up, maintains, and terminates the connection and handles synchronization between the two devices.
6. **Presentation Layer**: The presentation layer deals with the format of the data that is being transmitted. It handles the conversion of data between different formats and provides encryption and decryption services.
7. **Application Layer**: The application layer provides user-level services and interfaces with applications. It defines the protocols that applications use to communicate with each other.

This model allows developers to create protocols and applications that work together seamlessly and can be used across different hardware and software platforms.

![Screenshot 2023-05-01 213336](https://user-images.githubusercontent.com/118557513/235483836-365c2dca-35b0-4b0f-97d9-7aefbcf43636.png)

The picture above gives us a brief idea about what each layer deals with.
