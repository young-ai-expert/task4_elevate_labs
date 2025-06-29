# task4_elevate_labs
# Setting Up and Using UFW Firewall on Linux

## Objective

Configure and test basic firewall rules to allow or block traffic using UFW (Uncomplicated Firewall) on Linux.

## Steps

1.  **Enable UFW:**

    ```bash
    sudo ufw enable
    ```

2.  **Allow SSH Traffic (if necessary):**

    ```bash
    sudo ufw allow ssh
    ```

    Or, specify the port number:

    ```bash
    sudo ufw allow [port_number]/tcp
    ```

3.  **Block Inbound Traffic on a Specific Port (e.g., 23 for Telnet):**

    ```bash
    sudo ufw deny 23
    ```

4.  **Remove the Test Block Rule:**

    ```bash
    sudo ufw delete deny 23
    ```

5.  **Check UFW Status:**

    ```bash
    sudo ufw status verbose
    ```

## Summary

UFW filters network traffic by examining packets and comparing them against a set of rules. It allows or blocks traffic based on these rules.
