# Mullvad-Reminder
A simple systemd service opening a program if an output is some specified string. In this case, the Mullvad-VPN app is launched if the VPN is disabled.

The purpose is general use, if something is not set, launch a GUI app to remind you to set it. In this case, know you have the VPN disabled, quite agressively, instead of just the tray icon (lol Gnome)

currently not working, no idea why.

Install:

```
sudo wget https://github.com/trytomakeyouprivate/Mullvad-Reminder/raw/main/mullvad-reminder.service -o /etc/systemd/system/mullvad-reminder &&\
sudo systemctl enable mullvad-reminder && sudo systemctl start mullvad-reminder &&\
echo "Mullvad-reminder service enabled!"
```
