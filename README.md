# Thinkpad T480 Backlight on Boot Fix
This service fixes the issue T480s could face when booting, causing the keyboard backlight to be off even though the kbd_backlight/brightness value is set to 1, forcing the user to manually toggle it

## Copy the service file
```
sudo cp kbd-backlight-init.service /etc/systemd/system/
```

## Reload systemd
```
sudo systemctl daemon-reload
```

## Enable it to run on boot
```
sudo systemctl enable kbd-backlight-init.service
```

## Start it now to test without rebooting
```
sudo systemctl start kbd-backlight-init.service
```
