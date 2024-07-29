# This page will tell you the ways to install the display driver in different operating system  

# Raspberry Pi OS  

Add the following line in `/boot/config.txt` in your TF card  

```sh
dtoverlay=vc4-kms-dpi-hyperpixel4sq
``` 
And the `config.txt` file will look like this:  
![image](https://github.com/user-attachments/assets/33139e0d-2477-4732-8ff5-a3e2bce9d383)  
Now you can insert the TF card in to the slot and your HackberryPi will run Raspberry Pi OS on the screen.  

# Kali Linux    

### Step 1  
Add the following lines in `/boot/config.txt` in your TF card  

```sh
dtoverlay=hyperpixel4
overscan_left=0
overscan_right=0 
overscan_top=0
overscan_bottom=0
framebuffer_width=720
enable_dpi_lcd=1
display_default_lcd=1
dpi_group=2
dpi_mode=87
dpi_output_format=0x5f026
dpi_timings=720 0 20 20 40 720 0 15 15 15 0 0 0 60 0 36720000 4
```
### Step 2  
put the `hyperpixel4.dtbo` into `/boot/overlays`  
Now you can insert the TF card in to the slot and your HackberryPi will run Kali Linux on the screen.  
