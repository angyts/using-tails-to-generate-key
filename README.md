{% tabs %}
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

Download the official image from the [Tails website](https://tails.boum.org/install/index.en.html). Might take a while, go grab a coffee.

Make sure you follow the guide on the Tails website to verify your download of Tails.

### Part 2 - Download and install the software to transfer your Tails image on your USB stick

For Windows:
- [Etcher](https://tails.boum.org/etcher/Etcher-Portable.exe)
- [Win32 Disk Imager](https://win32diskimager.org/#download)
- [Rufus](https://rufus.ie/en_US/)

For Mac download [Etcher](https://tails.boum.org/etcher/Etcher.dmg)

### Part 3 - Making your bootable USB stick

Run the above software. This is an example how it looks like on Mac OS with etcher. But other software should be similar.

![](/assets/etcher_in_mac.png)

Select the Tails OS image that you downloaded as the image. Then select the USB stick (the larger one). 

Then flash the image to the larger USB stick.

### Part 4 - Download and verify the eth2-deposit-cli

You can refer to the other tab on this guide on how to download and verify the eth2-deposit-cli. 

Copy the file to the other USB stick.

### Part 5 - Reboot your computer and into Tails OS

After you have done all the above, you can reboot. If you are connected by a LAN cable to the internet, you can disconnect it manually.

Plug in the USB stick that has your Tails OS.

On Mac, Press and hold the Option key immediately upon hearing the startup chime. Release the key after Startup Manager appears. 

On Windows, it depends on your computer manufacturer. Usually it is by pressing F1 or F12. If it doesn't work, try googling "Enter boot options menu on [Insert your PC brand]"

Choose the USB stick that you loaded up with Tails OS to boot into Tails.

### Part 6 - Welcome to Tails OS

![](/assets/grub.png)

You can boot with all the default settings.

### Part 7 - Run the eth2-deposit-cli

Plug in your other USB stick with the `eth2-deposit-cli` file.

You can then open your command line into the directory containing the file. Then you can continue the guide from the other tab.

Make a new mnemonic.

```text
./deposit.sh new-mnemonic --chain mainnet
```

If you run this command directly from your other USB stick, the validator keys should stay on it. If it hasn't, copy the directory over to your non-Tails USB stick.

{% hint style="warning" %}
🔥**Make sure you have saved your validator keys directory in your other USB stick (non Tails OS) before you shutdown Tails. Tails will delete everything saved on it after you shutdown.**.
{% endhint %}

{% hint style="success" %}
🎉Congrats on learning how to use Tails OS to make an airgapped system. As a bonus, you can reboot into Tails OS again and connect to internet to surf the dark web or clearnet safely!
{% endhint %}

{% endtab %}
{% endtabs %}