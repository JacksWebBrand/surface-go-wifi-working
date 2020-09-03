Firmware change to make the ath10k  wifi on the Microsoft Surface Go (and other computers using the same wireless card) work in Linux. This is not a brand new fix, but it is the easiest way to go about it on the internet (that I can see). 

		- THIS -

- If you don't know which ath10k folder to place the updated bin file:
	1. REPLACE the 'ath10k' folder in /lib64/firmware/'ath10k' with the one from this repository.

			- OR -

- If you know which folder is the correct one for your exact wireless card:
	1. REPLACE the 'board.bin' file in the appropriate folder with the one from this repository.

(note you will need root access or sudo to make these changes)

		- DONE -

	- $ git clone https://github.com/JacksWebBrand/surface-go-wifi-working-linux.git
	- transfer the 'surface-go-wifi-working' folder to your Surface Go (or other computer) via usb, or some other way (or just clone direct with a usb->ethernet).
	- $ cd surface-go-wifi-working
	- $ sudo rm -rf /lib64/firmware/ath10k
	- $ sudo cp -r . /lib64/firmware

^ the above is the "I don't know which folder exactly to put it in" method. You only need to do one method, not both.

I WOULD RECOMMEND making a backup of your original ath10k folder first, for the usual reasons - problems can always get worse!
