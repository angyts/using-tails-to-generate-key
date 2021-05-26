{% tab title="Advanced - Most Secure" %}
{% hint style="warning" %}
🔥**\[ Optional \] Pro Security Tip**: Run the **eth2deposit-cli tool** and generate your **mnemonic seed** for your validator keys on an **air-gapped offline machine booted from usb**.
{% endhint %}

You will learn how to boot up a windows PC into an airgapped [Tails operating system](https://tails.boum.org/index.en.html).

The Tails OS is an *amnesic* operating system, meaning it will save nothing and *leave no tracks behind* each time you boot it.

### Part 0 - Prerequisites

You need:

- 2 storage mediums (can be USB stick, SD cards or external hard drives)
- One of them must be > 8GB  
- Windows or Mac computer
- 30 minutes or longer depending on your download speed 

### Part 1 - Download Tails OS

Download the official image from the [Tails website](https://tails.boum.org/install/index.en.html). 

Make sure you follow the guide on the Tails website to verify your download of Tails.

### Part 2 - Download and install the software to transfer your Tails image on your USB stick

For Windows:
- (Win32 Disk Imager)[https://win32diskimager.org/#download]
- (Etcher)[https://tails.boum.org/etcher/Etcher-Portable.exe]  
- (Rufus)[https://rufus.ie/en_US/]

For Mac download (Etcher)[https://tails.boum.org/etcher/Etcher.dmg]

### Part 3 - Making your bootable USB stick



{% embed url="https://www.youtube.com/watch?v=C97\_6MrufCE" %}

You can copy via USB key the pre-built eth2deposit-cli binaries from an online machine to an air-gapped offline machine booted from usb. Make sure to disconnect the ethernet cable and/or WIFI.
{% endtab %}
{% endtabs %}