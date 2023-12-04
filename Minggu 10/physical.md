
`Tugas ini merupakan tugas mata kuliah Konsep Jaringan yang dibimbing oleh Bpk. Dr. Ferry Astika Saputra,ST, M.Sc`

# Physical Design Mikrotik

Configurasi :

![image](https://github.com/Mahargip/Konsep-Jaringan/assets/114201452/9d8ca7bd-e06e-4206-ad50-2260f184ef0e)


## **1. Router 0**
    - Static
        Network     : 192.168.1.0
        Mask        : 255.255.255.0
        Next Hop    : 10.252.108.11
    - Fe 0/0
        IPv4 Address: 10.252.108.1
        Subnet Mask : 255.0.0.0

## **2. Router 1**
    - Fe 0/0
        IPv4 Address: 10.252.108.11
        Subnet Mask : 255.0.0.0
    - Fe 1/0
        IPv4 Address: 192.168.1.1
        Subnet Mask : 255.255.255.0

## **3. PC 0**
    IPv4 Address    : 192.168.1.2
    Subnet Mask     : 255.255.255.0
    Default Gateway : 192.168.1.1

## **4. PC 1**
    IPv4 Address    : 192.168.1.3
    Subnet Mask     : 255.255.255.0
    Default Gateway : 192.168.1.1

## **5. PC 2**
    IPv4 Address    : 192.168.1.4
    Subnet Mask     : 255.255.255.0
    Default Gateway : 192.168.1.1
