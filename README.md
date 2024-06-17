# openwrt-fireware-build
Build for xiaomi/Redmi AX6 with WiFi NSS drivers and turbo acc.  
Thanks and respect to TerryLip (https://github.com/TerryLip/AX6NSS)  

I'm on purpose to build an AX6 mini firmware  
without any applications (for instance, Passwall2 or OpenClash and some kinda "core" which requires large space)  
that need to be updated regularly.  
For my view, the AX6 has a small flash memory.  
The SquashFS will not release any space after you uninstall pre-built applications.  
Compiling those kinda large packages inside means "double space".  
So it would be better to compile a mini firmware  
then install the applications (like Passwall2 or OpenClash whatever) you want.  


reference:  
https://www.right.com.cn/forum/forum.php?mod=redirect&goto=findpost&ptid=8343458&pid=19765808


recommand:  
If you wanna compile an AX6 firmware,  
fork this repo,  then copy and edit this repo's AX6.config  
to be your own ./config/xiaomi_ax6-stock.config:  
https://github.com/TerryLip/AX6NSS

Mine may not match your desire.  
I had also encountered curl 55 errors with the firemware I compiled and had no idea what was going on.  
Stripped too much?

If you want a regular auto-build,  
check and analyze ./scripts/prepare.sh and ./.github/workflows/build-firmware.yml .  
(I was intend to do that but got pretty much lazy so.)
