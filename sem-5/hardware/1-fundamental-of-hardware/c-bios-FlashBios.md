**Basic Input Output System (BIOS) :**  
It provides a set of instructions and is responsible for booting the computer. The BIOS performs all the test needed at startup time. These tests are collectively known as Power On Self Test(POST) .The computer contains hardware like keyboard, monitor, disk drives, etc. there functioning requires interfacing with the operating system. The BIOS provides drivers for basic hardware like keyboard and monitor, mouse, etc. The operating system provides hardware for printer, modem, etc. Drivers for some hardware may not be available in the operating system hence these have to be explicitly installed by the user.

**Power On Self Test (POST) :**  
POST consists of a series of diagnostic test that runs automatically when a user turns on the computer. The actual test may differ depending on the configuration of the BIOS. However, the usual test includes testing of the RAM, keyboard and the disk drives. If these tests are successful the computer boots itself and loads the operating system but if these tests are unsuccessful, the computer reports the errors through a series of beeps to draw the operator’s attention and finally an error message is displayed on the monitor.

![](https://media.geeksforgeeks.org/wp-content/uploads/20200305183055/BIOS.jpg)

**Location Of BIOS :**  
BIOS is typically placed in a chip known as Read Only Memory(ROM) that comes with the computer. This ensures that the BIOS will always be available even if the hard disk is formatted or replaced. However, in many cases the content of the ROM is transferred to the RAM when the system is started. This is because the RAM allows quicker access as compared to the ROM. Copying of the content of the ROM to the RAM is known as shadowing.

**Complementary Metal Oxide Semiconductor RAM :**  
As the BIOS will interface the hardware with the operating system, it will require configurations of the hardware components like hard disk, monitor, etc. This information is permanently saved in an area known as Complementary Metal Oxide Semiconductor Random Access Memory (CMOS RAM). Power is supplied to the CMOS from a small battery so its contents will not be lost after the PC is turned off. Therefore, there is a battery and a small RAM memory on the board which stores information in a permanent manner. The CMOS needs very little power so there is not much of strain on the computer’s battery. Even then the battery is rechargeable is recharged every time the computer is turned on.

![How to Flash BIOS Settings on Windows PCs](https://store.hp.com/app/assets/images/uploads/prod/how-to-flash-bios-settings-on-windows-pcs-hero1570476493398462.jpg)

[HOME](https://www.hp.com/us-en/shop/tech-takes)

# How to Flash BIOS Settings on Windows PCs
Your computer’s BIOS is an integral part of making sure your PC starts and runs correctly. If you’ve been experiencing issues with starting up your computer, you may have read that you should flash the BIOS. What does it mean to do this? Is it safe?

Here is what you need to know about this task and whether you even need to do it at all. It might be that you simply need to replace your CMOS battery ([read how to do that here](https://www.hp.com/us-en/shop/tech-takes/what-is-cmos-battery-how-to-remove-and-replace)) or you may need to replace a corrupted driver. If you do need to flash the BIOS, we can help. Read on for tips to get you up and running again.

## What does it mean to flash a BIOS?

For your computer to start up (also known as "booting up"), it needs instructions. These instructions are stored in the Basic Input/Output System, or BIOS. If your BIOS isn't updated, it's possible that your computer could have difficulty performing basic tasks, such as interacting with your hardware and making sure the operating system runs quickly and without bugs - especially upon startup.

If you run into issues getting your computer to boot up properly, it may be a BIOS problem. “Flashing the BIOS” is a term used by computer-savvy people to describe the process of updating the BIOS.

## Is it safe to flash BIOS?

If you know what you’re doing or are relying on automatic updates from your PC manufacturer, this can be an easy and effective way to get a buggy PC working smoothly again. If you’re not confident with manually adjusting the BIOS settings or are unsure if your problem is related to the BIOS, you may want to leave the manual update to an expert. There’s also a danger to your computer if you experience a shut-down or frozen PC during the BIOS update. A BIOS update that doesn’t complete can cause more harm than good.

Getting familiar with your BIOS menu and settings is a practical first step to learning how to flash BIOS. Note that Mac computers do not have a BIOS.

## Flashing BIOS through an automatic update

Fortunately, most HP computers will update the BIOS as part of their regular updates. To see if your computer needs an update, do the following:

-   Search for the  **HP Support Assistant**  and open it
-   Click on the  **My devices**  tab
-   Find your computer and choose  **Updates**
-   Choose  **Check for updates and messages**
-   If you need a BIOS update, a checkbox will appear next to the  **BIOS update**  field. Check it, along with any other updates you want to be done, and choose  **Download and install**

## How to check BIOS version for manual updates

What about computers not made by HP®? Flashing a BIOS merely means to update it, so you don’t want to do this if you already have the most updated version of your BIOS. But how can you tell what you have? You can check the BIOS version you are running in one of the following ways:

1.  Click  **Windows+R**  to open the run box, type “**msinfo32**,” and hit  **Enter**. The system information window will open for you to see the BIOS version/date number in the System Summary
2.  Open a Command Prompt window by typing “**cmd**” in the Windows search box. When opened, type the following:  **wmic bios get smbiosbiosversion** (The current version will appear)

## History of BIOS

[BIOS](https://www.geeksforgeeks.org/introduction-of-basic-input-output-system-bios/)  was first introduced in 1975, in CP/M Operating System. Control Program for  [Microcomputers](https://www.geeksforgeeks.org/introduction-of-microcomputer-system/), was developed for Intel 8080/85-based microcomputers by Gary Kildall of Digital Research, Inc. The system had a simple bootloader in its ROM.  
IBM classified the system bios into two categories when PS/2 machines were introduced:

-   **CBIOS:**  CBIOS stands for  **Compatibility BIOS**. The real-mode portion provided backward compatibility with current operating systems and thus was named CBIOS.
-   **ABIOS:**  ABIOS stands for  **Advanced BIOS**. It provided new interfaces, especially the one suited for multitasking OS.

## Functions of BIOS

-   **POST:** Power on Self-Test is the process performed by BIOS immediately after the computer system starts to check any hardware-related issues. if any error is found in this process, the system alerts through flashing LEDs, audible beeps, or error messages on the monitor, all of which are technically referred to as POST codes, beep codes, and on-screen POST error messages, respectively.
-   **Bootstrap Loader:**  The bootstrap program stored in ROM is loaded in the hard drive, as soon as the computer starts. The bootstrap loader locates the operating system and passes the control to it.
-   **Bootstrap Driver:**  Bootstrap Driver configures basic hardware so that system can run. They are low-level drivers and give basic information about computer hardware.
-   **CMOS Setup:**  [Complementary Metal-Oxide Semiconductor(CMOS)](https://www.geeksforgeeks.org/what-is-cmos-fabricationp-well-process/)  chip, saves some system information, such as the time, date, and other essential system settings. CMOS chip is powered by the battery located in the motherboard. It also stores some information about hardware. The chip’s content is copied to the RAM(main memory) of the system to increase the speed since the CMOS chip is quite slow. It is because the BIOS and CMOS, setup configure the system’s crucial information like the password, date, and time.
-   **Boot device selection:**  One of the CMOS’s most important roles is, it can alter the device boot process. This is important for system restoration because the CMOS may need to change boot priority from the hard drive to the optical drive or flash drive to launch the operating system installer or adjust which hard drive to load the operating system from.

## Working of BIOS

A basic Input/Output System (BIOS) is a kind of program that can be accessed by the  [EPROM (Erasable Programmable Read Only Memory)](https://www.geeksforgeeks.org/difference-between-eprom-and-eeprom/)  chip. Upon switching on the system, the control is passed to BIOS Program in a similar place on EPROM.

The main work of the BIOS is that it checks whether each and every important attachment are in the right place or not. When it is checked that all boot devices are properly working, BIOS has the work to load Operating System.

![Working of BIOS](https://media.geeksforgeeks.org/wp-content/uploads/20230529091021/BIOS-Full-Form-660.png)


### **Fundamental Services of BIOS:**

-   **POST:** [POST](https://www.geeksforgeeks.org/what-is-post/)  checks your PC’s hardware and ensures that nothing is out of order and that your operating system is error-free. POST checks everything from your keyboard and disc drive to your computer’s RAM speed and integrated ports. If everything is in order, POST will continue as usual and your PC will boot normally. If an error is detected, BIOS will generate an error message, which may take the form of displayed text or a series of error-indicating beeps. These beeps are always signals for specific messages, so if you get this result, you should investigate what it means for your computer’s hardware.
-   **CMOS setup:** Within its  [CMOS](https://www.geeksforgeeks.org/bios-full-form/), your computer stores all low-level settings such as system time and hardware configuration. This means that any changes you make to the structure of your BIOS are saved on a special memory chip known as the Complementary Metal-Oxide Semiconductor, or CMOS. The CMOS setup is in charge of configuring your password, time, and date.
-   **Bootstrap loader:** The [bootstrap loader](https://www.geeksforgeeks.org/booting-and-dual-booting-of-operating-system/) is a program that lives within your computer’s  [EPROM](https://www.geeksforgeeks.org/eprom-full-form/)  or  [ROM](https://www.geeksforgeeks.org/read-only-memory-rom/)  and is tasked with reading your PC’s hard drive boot sector in order to complete the operating system load. The bootstrap loader activates the POST and then loads Windows 10 into memory when you restart your computer.  [UEFI](https://www.geeksforgeeks.org/uefiunified-extensible-firmware-interface-and-how-is-it-different-from-bios/), or Unified Extensible Firmware Interface, has replaced the bootstrap loader in newer PCs.

## Features of BIOS

-   Every BIOS implementation is specifically designed for a particular type of motherboard model or particular computer.
-   Originally, BIOS firmware was stored in the ROM memory but nowadays it is stored in Flash memory so that it can be rewritten without removing the chip from the motherboard.
-   The other reason for doing this is that it allows easy updates of BIOS firmware, so new features can be added and bugs can be fixed.
-   The latest advancement of BIOS is  [UEFI(Unified Extensible Firmware Interface)](https://www.geeksforgeeks.org/uefiunified-extensible-firmware-interface-and-how-is-it-different-from-bios/).

## Accessing BIOS

With BIOS, many computer applications are not having any restrictions to keep the details of the hardware, attached I/O device, etc. Consumers have access to BIOS and also the configuration of BIOS. Some of the steps mentioned below help in setting up the BIOS.

## How to Setup BIOS?

**Step 1:** First turn off your computer or simply restart it.

**Step 2:**  When the system turns On, wait for the message similar to ‘entering setup’ to come.

**Step 3:**  Wait for the message ‘Press Key to enter BIOS Setup’. Some keys are like Del, Tab, etc.

**Step 4:**  Press the specified key as early as possible.

**Step 5:**  Process Complete.

## BIOS Security

BIOS Security is an advanced feature of cybersecurity. It has the work to protect the Operating System from suspicious activities. Plundervolt is one of the manipulations of BIOS which is used to manage computer power supply at the time of memory writing, that has the work to maintain the security gaps which overall results in improving the security of the BIOS.

## BIOS Manufacturers

IBM was the first organization that single-handedly owed the BIOS. In spite of IBM, there were several other companies like Phoenix Technologies have their own BIOS. There are several companies that are producing motherboards with embedded BIOS chips in them. Some of the companies are HP, Ricoh, etc. Each organization has its own drivers of motherboards, and each of them creates it in a unique way.

## Advantages of BIOS

-   The computer system will gain better compatibility.
-   The booting time of the system decreases.
-   The overall performance of the system improves.

## Disadvantages of BIOS

-   The disadvantage is that it is a time-consuming process. BIOS often boots in 16-bit real mode (not 32-bit nor 64-bit protected mode), and because of the type of chip used, it is not always the fastest.
-   If something goes wrong during the process, the motherboard might get affected. Solving this will not be an easy process.

## Update
### **Simple Level Method (Windows Update):**

Some manufacturers, such as HP, will provide BIOS updates via their own software update utilities. This makes updating much easier because you don’t have to enter the BIOS setup before running the update. Others, such as Acer, will necessitate the downloading of an EXE file from the manufacturer’s website. Instead of rebooting your computer, simply double-click the update program, and it will perform the reboot and update process for you. In any case, you should still enter the BIOS setup before running the update to make a note of any settings you want to keep. Once the process is complete, and you’ve made any necessary settings changes, you can resume using your computer as usual, with whatever improvements or fixes the BIOS update provided.
### **Intermediate Level Method (Download the Update):**

Navigate to the Support page for the manufacturer of your PC, such as Dell, HP, or Lenovo. Then, look for the support page for your specific PC by searching for the model number or serial number, which is usually located somewhere on the device. (If you built your own PC, look for the motherboard manufacturer, such as Asus, Gigabyte, or MSI.) When you get to the Support page, look for a section for downloads or drivers.  
Go there and look for BIOS or UEFI updates.

### **Advance Level Method (Format a Flash Drive):**

Many PCs (especially older ones) will require you to format a flash drive, copy the new BIOS file to it, and reboot your computer while pressing a key to enter the BIOS setup (frequently Delete, F2, or another key you’ll see on-screen at boot). Once inside the BIOS, make a note of any previous changes you’ve made, as an update will typically reset your system to the default settings. If you need to remember your setup, take photos of each category. Then, look for the option to update your  [firmware](https://www.geeksforgeeks.org/difference-between-hardware-and-firmware/), and you’ll be able to use the file on your flash drive to run the update utility.  
If you interrupt the process or turn off your computer during this time, your computer may become unusable.
