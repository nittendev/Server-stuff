# Dell R720 IDRAC Commands

Manual commands to issue fan speed commands to dell idrac systems like the R720

##Enable manual control:
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x01 0x00

##setting speed:
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x02 0xff 0x14

##Set fan speed to 25%
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x02 0xff 0x19
Set fan speed to 30%
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x02 0xff 0x1E
Set fan speed to 50%
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x02 0xff 0x32
Set fan speed to 60%
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x02 0xff 0x3C
Set fan speed to 100%
ipmitool -I lanplus -H SERVERS_IP_HERE -U IDRAC_USERNAME -P 'IDRAC_PASSWORD_HERE' raw 0x30 0x30 0x02 0xff 0x64
