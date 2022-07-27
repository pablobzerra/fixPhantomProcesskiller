#!/bin/bash

argv=$1
ip=$(ifconfig | grep "192.168.0." | awk '{ print $2 }')
function main() {
echo "---------------------------"
echo "    FixPhantom-Process"
echo "---------------------------"
echo "[ IP ]: "$ip
echo "[ PORT ]: "$argv
echo "---------------------------"
fix_phantom
}

function fix_phantom() {
{
adb connect $ip:$argv > /dev/null
adb shell /system/bin/device_config put activity_manager max_phantom_processes 2147483647 && echo "[ INFO ]: SUCESSO✓"
} || {
#clear
echo "[Error]: Ocorreu um problema ao remover o phantom"
}
}
main
