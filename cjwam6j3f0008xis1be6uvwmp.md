## Run Fast Android Emulators with Intel HAXM

%[https://www.youtube.com/watch?v=7I4upqY0H4M&t=34s]

Now you can accelerate Android Emulator in Visual Studio using Intel Hardware Acceleration Execution Manager for x86 images!

Steps to follow:

1. Open CMD as administrator
2. Disable Hyper-V by entering “bcdedit /set hypervisorlaunchtype off”
3. Restart your PC
4. Install Intel HAXM from Visual Studio Installer or manually from [here](https://github.com/intel/haxm/releases) 
5. After install, run any Xamarin Android project on x86 based emulator. You will see how fast the emulator will load because now it’s running with Intel HAXM.

###### Note: ***Intel HAXM only work with Intel CPU that supports Intel VT-x.***

[Does My Processor Support Intel® Virtualization Technology?](https://www.intel.com/content/www/us/en/support/articles/000005486/processors.html) 

[Visit Full Guide](https://docs.microsoft.com/en-us/xamarin/android/get-started/installation/android-emulator/hardware-acceleration?pivots=windows#accelerating-with-haxm) 

*****
###### **Keep learning and Enjoy!**