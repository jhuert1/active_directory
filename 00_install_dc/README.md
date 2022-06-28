# 01 Install Domain Controller

1. Use 'sconfig' to:
    - Change the hostname
    - Update IP address and set as static
    - Change DNS server to our own IP address

2. Install Active Directory Feature
    - (Shell) Install-WindowsFeature AD-Domain-Services -IncludeManagementTools