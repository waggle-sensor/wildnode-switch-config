# Wild Waggle Node Unifi Network Switch Config

This repo contains a copy of the firmware and configuration for the [Unifi EdgeSwitch 8 150W](https://store.ui.com/collections/operator-edgemax-switches/products/edgeswitch-8-150w)

> The firmware and config are used by [surya-tools](https://github.com/waggle-sensor/surya-tools) when preparing the Wild Waggle Node network switches.

# Creating the Switch Config

These are the steps that are taken to create the network switch config:

1. Login to an existing node to get access to the network switch web UI

    ```bash
    ssh -L 9191:10.31.81.2:443 node-<node id>
    ```

2. Switch to the "new UI" (if it is not already set).
3. Click the "System Settings" tab, click "Backup" under "System Actions"
4. Safe the *.tar.gz file and rename to `waggle_config_v<version>.tar.gz`
5. Replace the existing config (`./config`)
