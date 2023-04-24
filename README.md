# Mullvad-Reminder
A simple systemd service opening a program if an output is some specified string. In this case, the Mullvad-VPN app is launched if the VPN is disabled.


Install:

```
sudo wget https://github.com/trytomakeyouprivate/Mullvad-Reminder/raw/main/mullvad-reminder.service -o /etc/systemd/system/mullvad-reminder &&\
sudo systemctl enable mullvad-reminder && sudo systemctl start mullvad-reminder &&\
echo "Mullvad-reminder service enabled!"
```
