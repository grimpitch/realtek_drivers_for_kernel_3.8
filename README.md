Updated Realtek drivers for kernel version 3.8
==============================================

This driver source package is modified to be able to compile on the version 3.8 linux kernel branch.

1. The supported Realtek wireless adapters and device IDs are the following:

    RTL8188CE/RTL8192CE		8191, 8178, 8177, 8176
    
    RTL8192DE		    	8193, 002B
    
    RTL8191SE/RTL8192SE		8192, 8171, 8172, 8173, 8174
    
    RTL8188EE			    8179
    
    RTL8723AE		    	8723

2. Compile & install

Change to the directory of the driver and issue the following commands as super user (root):

    make
    make install

3. Load the module

You can load the appropriate module for your card by executing:

    modprobe module_name

where module name can be:

    rtl8192ce, rtl8192de, rtl8192se, rtl8188ee, rtl8723e

depending on your wireless chip.
