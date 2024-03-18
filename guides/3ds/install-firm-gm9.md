# Installing FIRM with GodMode9

This page is only really for edge-case situations. For example:
* Troubles with SafeB9SInstaller ('`FIRM backup fail`', stuck on checking (micro)SD card, etc?)
* A blender of a CFW setup (but you at least know how to get into GodMode9)

If you stumbled upon this page from a Google search(!?!?), please [try install boot9strap normally](https://3ds.hacks.guide) first. <br/>
If you have any troubles with it, *consult the troubleshooting sections or ask for help*. Please don't use this page as a second resort.

## Prerequisites
- Your 3DS in GodMode9. **NOTE: Installing FIRM files was only added in GodMode9 v1.4.0.**
- An SD card in your 3DS.
- A FIRM to install.
	- For example, [boot9strap](https://github.com/SciresM/boot9strap/releases/latest){:target="_blank"}, or [fastboot3DS](https://github.com/derrekr/fastboot3DS/releases/latest){:target="_blank"}.

## Instructions

### Preparing files

**💡 TIP:** If you are currently in GodMode9, press R+B to unmount your SD card before ejecting it.

1. Copy the `.firm` file to a location on your SD card. (This can be anywhere, just make it easy to find.)
1. Safely eject your SD card from your PC.

### Installing FIRM

1. Insert your SD card into your 3DS and load up GodMode9.
1. Select `[0:] SDCARD` and find the `.firm` file you have placed on it.
1. Select the file, then select `FIRM image options... -> Verify File`.
1. If the resulting screen says `Verification Success`, press `(A)` to continue. <br/>
If it does NOT say verification succeeded, **STOP.** Copy the file to your SD card again.
1. Select the `.firm` file again, then select `FIRM image options... -> Install FIRM`.
1. You will be prompted to unlock SysNAND lvl3 writing. Follow the on-screen prompt.
1. Press (START) to reboot your console.

If the SysNAND lvl3 writing prompt scared you, then that's great!
As of this writing, there have been `3` incidents of users installing [finalize_helper.firm](https://3ds.hacks.guide/finalizing-setup){:target="_blank"} to FIRM with no remorse.

In the event this happens to you, download a normal build of GodMode9 (or, the [SafeB9SInstaller](https://github.com/d0k3/SafeB9SInstaller/releases/latest){:target="_blank"}) and put it on your SD card as `iderped.firm`.
(See: [GodMode9/arm9/source/godmode.c#3083-3085](https://github.com/d0k3/GodMode9/blob/master/arm9/source/godmode.c#L3083){:target="_blank"}.)

