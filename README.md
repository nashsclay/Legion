# Legion Coin Masternode Setup
This Legion Coin Masternode (MN) script will automatically install almost all of the MN for you. You just need to have your masternode genkey ready. This code comes from Zoldurs many many forks for MN scripts, visit his page here. https://github.com/zoldur<br /><br />
Please note to run this script you MUST:
1) Be root - better to login as root then use the sudo command
2) Ubuntu 16.04 - I only tested this on that version but I'm sure others may work.
3) A VPS server - You can use my referal link here --> https://www.vultr.com/?ref=7415368
4) Digital Ocean is another provider you can use instead of Vultr. There are many more but these are very common to use. You can use any size due to the swap file that will be created if your server is below 2GB of memory.
5) Optional - There may be other types of servers you can use but not listed here.
legion_mn_setup_1.0.0_swap.sh<br />

Do note that this script does enable the MN to restart if it is somehow closed. It will only make it difficult to remove the MN if you decide to sell your MN. Best way is to delete all the MN files and to restart the MN. (for more information, please vist the coin's discord)

## To Install the Legion Coin Masternode

Go through setting up the wallet and MN infomration on your computer. Then once that is ready to go, continue on to this guide. 

Please copy and paste the following commands into you connection with your server. Most common would be to use Putty.
NOTE: Don't click on the links as that will only show you code. There is no need to do so.

> wget https://raw.githubusercontent.com/nashsclay/Legion/master/legion_mn_setup_v1.0.sh<br />
> chmod +x legion_mn_setup_v1.0.sh<br />
> ./legion_mn_setup_v1.0.sh<br />


### Other Commands and Informaiton
This information will be very useful once your MN is setup and ready.

Displays currention information about the masternode
> legiond getinfo<br />


You want to see a 9 and that will show your Masternode is ready to go.
> legiond masternode status<br />


Will stop your masternode and wil automatically restart
> legiond stop<br />


This will allow you to edit your masternode's wallet (not your computer's wallet). You can also you this command after the setup to fix if you input the incorrect MN key. Once open and done making changes, press Ctrl + o then Enter to save changes, then Ctrl + x to exit. Then run the legiond stop to restart the MN.

> nano ~/.Legion/Legion.conf<br />


This is where your legiond file is saved to
> cd /usr/local/bin<br />


Return to root home folder
> cd ~<br />


This will give you access to the folder of Legion files. Notice the period infront of the folder. If your are in the home folder and do **ls** command, it will not show the folder. Period means hidden. Correct command to display this folder in the home folder is **ls -al**
> cd ~/.Legion<br />


Any donations are always welcome but never expected.
Legion - LSyPBnDJrBsVMN1j8EK1NA1QbUh8tx62Ao

You can alway DM me on discord at nashsclay#6809
