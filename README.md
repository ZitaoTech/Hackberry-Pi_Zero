# Hackberry-Pi_Zero
A handheld Linux terminal using Raspberry pi Zero 2W as Core with 4' 720X720 TFT display
### [Questions or need more info? Join my Discord Channel!](https://discord.gg/WzPthAmMbP)  
# <a name='About this handheld  '>About this handheld   </a>
The main reason why I design and build this handheld cyberdeck is to treat this as a lernning tool and also a funny toy for the hackers. It is powered by a raspberry pi zero 2w and a 4' 720X720 TFT display. 

Here are some **main Features:**  
**Main Processor**: Only compaticable with Raspberry pi zero 2w.  
**Display**: 4' 720X720 high resolution TFT display.  
**Dual Swapable battery Design**: Replace your battery in 10 seconds without killing the power!  
**Battery type**: Nokia BL-5C. You can buy it anywhere in the world.  
**Battery life**: In my test: 3.5 hours with desktop, 5 hours with commandline.  
**Keyboard Mouse Combo**: Yes, this cyberdeck has keyboard and mouse combo on board. You can choose blackberry Q10 or Q20 keyboard.  
**Fully customizable keymap**: You can connect the keyboard with a computer and customizable the keymap through [VIAL](https://get.vial.today/) easily.  
**3 USB2.0 Ports**: This handheld has 3 USB2.0 Ports, you can use it with USB-Stick or 4G Modul Dongle or any USB thing.  
**Charging Ampere**: 1A charging ampere, this handheld can be fully charged within 3 hours.  
**Stemma I2C Port**: This device has a stemma I2C port on board, you can connect with any I2C sensors.  
**TF card Slot**: There is an external TF card Slot. You can replace your OS image very easily.  

## Block Diagram
![Blockdiagramm_HackberryPi_Zero](https://github.com/user-attachments/assets/e46c354c-9363-41e2-b276-73ba5900a178)


# <a name='Get started  '>Get started   </a>
### How to turn on the HackberryPi?  
Turn the red switch to the **right position** and then press the **red button** to the left side of the red switch to power the USB Hub Controller Chip otherse the keyboard **can't be used!** At the same time the indicator for the battery voltage will be turned on.    
![Turnon](https://github.com/user-attachments/assets/9e333c90-5131-4404-85bd-e2c72a7e1bd3)  
![turnon](https://github.com/ZitaoTech/Hackberry-Pi_Zero/blob/main/Picture/Turnon.gif)
# <a name='Keyboard  '>Keyboard   </a>
The keyboard type is blackberry Q10 or Q20 keyboard. Both have the same keyboard layout.  
There is a red switch on the left side to decide if the keyboard controller communicates with the HackberryPi or with other device through the USBC-Port underneath.  
The idea about this is you can connect the keyboard with your computer and customize the keymap using [VIAL](https://get.vial.today/) or the handheld can be used as an emergency keyboard mouse combo.  
![keyboard](https://github.com/user-attachments/assets/63ac5772-f248-4117-bd29-ae0b3058e1e4)
### How to change the keymap?  
Put the red switch to the lower position, connect the keyboard with your computer, open [VIAL page](https://vial.rocks/), then you can customize the keymap yourself.  
![image](https://github.com/user-attachments/assets/7c4e9b53-7a00-4cdd-b0b7-751647f76f6b)


# <a name='Different Operating System  '>Different Operating System   </a>
You can install Kali, Raspberrypi OS, or Retropi and many other OS into HackberryPi.
# <a name='Basic Tutorial  '>Basic Tutorial   </a>
虚拟环境pip
[tiptop](https://github.com/nschloe/tiptop)+[recn](https://stackoverflow.com/questions/75602063/pip-install-r-requirements-txt-is-failing-this-environment-is-externally-mana)  
[TUI](https://terminaltrove.com/new/) apps in Terminal:  
[Web browser](https://itsfoss.com/terminal-web-browsers/) in Terminal:  
How to increase [swap](https://pimylifeup.com/raspberry-pi-swap-file/) on a raspberry pi  

Lightweight Web browser: [Midori](https://pimylifeup.com/raspberry-pi-midori/) 
![image](https://github.com/ZitaoTech/Hackberry-Pi_Zero/assets/145678024/f2de97d5-83dc-4a09-9b0d-42864c40fca8)


How to enable [mouse](https://www.youtube.com/watch?v=hycfIoGggjw&ab_channel=RickMakes) in Terminal
```shell
sudo apt install gpm
```
coding remote on [VSCODE](https://randomnerdtutorials.com/raspberry-pi-remote-ssh-vs-code/)

How to change font size in [terminal](https://askubuntu.com/questions/173220/how-do-i-change-the-font-or-the-font-size-in-the-tty-console)

屏保:[CMATRIX](https://www.raspberrypi-spy.co.uk/2013/01/matrix-pi-running-cmatrix-on-the-raspberry-pi/)
