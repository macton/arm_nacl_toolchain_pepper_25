arm_nacl_toolchain_pepper_25
============================
Pre-built Native Client (NaCl) linux_arm_newlib and linux_x86_newlib gcc toolchains and libs for ARM host.

STEPS TO INSTALL
----------------
* $(NACL_SDK) is wherever you installed nacl_sdk. See: https://developers.google.com/native-client/sdk/download
* $(ARM_TOOLCHAIN) is the directory this file is in.

* Go to the toolchain location
** $ cd $(NACL_SDK)/pepper_25/               

* The pre-installed toolchain is for x86 hosts only
** $ mv toolchain toolchain.x64              

* Decompress the arm toolchains 
** $ tar xzvf $(ARM_TOOLCHAIN)/toolchain.tgz 

Done. You can now build NaCl projects normally on your arm host.


NOTES ON BUILDING TOOLCHAIN
---------------------------
For notes on building toolchain from source on an ARM host, see thread: https://groups.google.com/d/topic/native-client-discuss/oTSZsUv8woM/discussion


NOTES ON DEVELOPMENT ENVIRONMENT
--------------------------------
I am running a Samsung ARM Chromebook in developer mode with an ArchLinux userspace installed on an external sdcard.
For notes on that process see: https://gist.github.com/4632677


@mike_acton
