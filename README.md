# Linux Scripts and Commands

Notes on usefull commands in linux

## Low volume iPods

```sh
sudo nano /lib/systemd/system/bluetooth.service

// change
ExecStart=/usr/lib/bluetooth/bluetoothd

// to
ExecStart=/usr/lib/bluetooth/bluetoothd --plugin=a2dp

// then
sudo systemctl daemon-reload
sudo systemctl restart bluetooth
```
