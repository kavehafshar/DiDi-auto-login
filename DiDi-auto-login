#!/bin/bash


USERNAME=""
PASSWORD=""


TARGET_WIFI="DiDi-UK"

CURRENT_WIFI=$(nmcli -t -f active,ssid dev wifi | grep '^yes' | cut -d':' -f2)

if [ "$CURRENT_WIFI" == "$TARGET_WIFI" ]; then
    echo "you are connected to didi"
    curl -X POST -d "username=$USERNAME&password=$PASSWORD&popup=true&dst= " https://wifi.didi.ir/login


else
    echo "sorry where is didi?"
fi
