# Subnetting

Konfigurasi : 

![image](https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/345eb68b-c1fe-418b-ab9f-382b9d53bcf7)

## **1. Router 0**
    - Static
        Network     : 192.168.1.0
        Mask        : 255.255.255.192
        Next Hop    : 192.168.10.14
    - Static
        Network     : 192.168.3.0
        Mask        : 255.255.255.240
        Next Hop    : 192.168.10.9
    - Fe 0/0 (ke Router 2)
        IPv4 Address: 192.168.10.13
        Subnet Mask : 255.255.255.252
    - Fe 1/0 (ke Router 1)
        IPv4 Address: 192.168.10.10
        Subnet Mask : 255.255.255.252
    - Fe 6/0 (ke Switch -> PC)
        IPv4 Address: 192.168.4.1
        Subnet Mask : 255.255.255.192

## **2. Router 1**
    - Static
        Network     : 192.168.4.0
        Mask        : 255.255.255.192
        Next Hop    : 192.168.10.10
    - Static
        Network     : 192.168.1.0
        Mask        : 255.255.255.240
        Next Hop    : 192.168.10.5
    - Fe 0/0 (ke Router 0)
        IPv4 Address: 192.168.10.9
        Subnet Mask : 255.255.255.252
    - Fe 1/0 (ke Router 2)
        IPv4 Address: 192.168.10.6
        Subnet Mask : 255.255.255.252
    - Fe 6/0 (ke Switch -> PC)
        IPv4 Address: 192.168.3.1
        Subnet Mask : 255.255.255.192

## **3. Router 2**
    - Static
        Network     : 192.168.4.0
        Mask        : 255.255.255.192
        Next Hop    : 192.168.10.13
    - Static
        Network     : 192.168.2.0
        Mask        : 255.255.255.224
        Next Hop    : 192.168.10.1
    - Static
        Network     : 192.168.3.0
        Mask        : 255.255.255.192
        Next Hop    : 192.168.10.6
    - Fe 0/0 (ke Router 0)
        IPv4 Address: 192.168.10.14
        Subnet Mask : 255.255.255.252
    - Fe 1/0 (ke Router 1)
        IPv4 Address: 192.168.10.5
        Subnet Mask : 255.255.255.252
    - Fe 6/0 (ke Router 3)
        IPv4 Address: 192.168.10.2
        Subnet Mask : 255.255.255.252
    - Fe 7/0 (ke Switch -> PC)
        IPv4 Address: 192.168.1.1
        Subnet Mask : 255.255.255.240

## **4. Router 3**
    - Static
        Network     : 192.168.1.0
        Mask        : 255.255.255.240
        Next Hop    : 192.168.10.2
    - Fe 0/0 (ke Router 2)
        IPv4 Address: 192.168.10.1
        Subnet Mask : 255.255.255.252
    - Fe 1/0 (ke Switch -> PC)
        IPv4 Address: 192.168.2.1
        Subnet Mask : 255.255.255.224


## **5. PC 0**
    IPv4 Address    : 192.168.4.3
    Subnet Mask     : 255.255.255.192
    Default Gateway : 192.168.4.1

## **6. PC 1**
    IPv4 Address    : 192.168.3.3
    Subnet Mask     : 255.255.255.192
    Default Gateway : 192.168.3.1

## **7. PC 2**
    IPv4 Address    : 192.168.1.3
    Subnet Mask     : 255.255.255.240
    Default Gateway : 192.168.1.1

## **8. PC 3**
    IPv4 Address    : 192.168.2.3
    Subnet Mask     : 255.255.255.224
    Default Gateway : 192.168.2.1
