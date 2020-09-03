Firmware change to make the ath10k  wifi on the Microsoft Surface Go (and other computers using the same wireless card) work.

1. If you don't know which ath10k folder to place the updated bin file:
	- REPLACE the 'ath10k' folder in /lib64/firmware/'ath10k' with the one in this repository.

2. If you know which folder is the correct one for your exact wireless card:
	- REPLACE the 'board.bin' file in the appropriate folder with the one from this repository.

(note you will need root access or sudo to make the above changes)

- $ cd surface-go-wifi-working
- $ sudo rm -rf /lib64/firmware/ath10k
- $ sudo cp . /lib64/firmware

^ the above is the "I don't know which folder exactly to put it in" method. You only need to do one method, not both.
