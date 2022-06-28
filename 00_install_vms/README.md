#00 - Install VMs

1. Installed Windows Server 2022 VM without GUI
2. Installed Windows 11 VM bypassing TPM
    a.  Press Shift + F10 to open Command Prompt and run the “regedit” command
    b. Add a new key in the “Setup” key
       In the Registry Editor, navigate to Computer\HKEY_LOCAL_MACHINE\SYSTEM\Setup. Right-click on the “Setup” folder in your sidebar and select “New > Key”.

    c. Name the key “LabConfig” and add a new DWORD
       After you name your folder, you can create the DWORD by right-clicking in any blank space in the main pane and selecting “DWORD (32-bit) Value”.

    d. Name the value “BypassTPMCheck” and set the value data to 1.
       It’s important the capitalization and spelling are exactly the same. You can modify the value data by double-clicking your new DWORD and changing the “Value data” text box. Press “OK” when you’re done to save the changes.

    e. Create another DWORD called “BypassRAMCheck”
       Again, make sure the capitalization and spelling is exactly the same as above.

    f. Change the value data to 1
       Remember, you can access the value data field by double-clicking on the “BypassRAMCheck” key. Press “OK” to apply it.

    g. Create a new DWORD called “BypassSecureBootCheck”

    h. Change the value data of SecureBootCheck to 1 and press “OK”

    i. Close the Registry Editor and press the back button on your Windows 11 setup

    j. Install Windows 11 on your unsupported hardware
       You can now go through the setup process as normal. Your installer should no longer tell you your PC is incompatible.
3. 