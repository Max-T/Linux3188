Linux3188

=========

Linux Source - RK3188 - PicUntu


Andy, from rikomagic has done it again


Finally wifi (MT5931) and Bluetooth (MT6622) are working on:
- iMito




----------------------

Just compile the kernel and build modules:
drivers/bluetooth/hci_uart.ko
drivers/mtk_wcn_bt/bt_hwctl.ko
drivers/net/wireless/mt5931/wlan.ko

place firmware under:
/system/etc/firmware/WIFI_RAM_CODE
/system/etc/firmware/MTK_MT6622_E2_Patch.nb0

FOR BLUETOOTH:
Build also hciattach from:
https://github.com/usumfabricae/MT6622_hciattach

