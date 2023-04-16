Now I want to add the changes to make the stock Sofle build work for the SofleRGB.
 I will need to add the following: 
 <myGithubAccountName>/zmk-config/config/ boards/shields/SofleRGB/Kconfig.defconfig // Defines split or not 
 boards/shields/SofleRGB/Kconfig/shield // More defines for shields 
 boards/shields/SofleRGB/SofleRGB.conf // Use this to define display=y/n and encoders=y/n 
 boards/shields/SofleRGB/SofleRGB.dtsi // Shield transforms. Define your rows and columns. 
 boards/shields/SofleRGB/SofleRGB.keymap // This is the keymap 
 boards/shields/SofleRGB/SofleRGB.zmk.yml // Not sure if I needed this. 
 boards/shields/SofleRGB/SofleRGB_left.overlay // define the perside columns. 
 boards/shields/SofleRGB/SofleRGB_right.overlay // define the perside columes

Once this built, I sent it to the board and had sucess. It is time to get this going for the Dactyl Manuform. Make a new folder and copy the files into that folder.
Then change all the references of SofleRGB to Dactyl. Alter the files to match the new shield. Done!