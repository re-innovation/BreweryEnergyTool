# BreweryEnergyTool
A tool for analysing the energy used in the brewing process.

This tool has been deeloped for accurately investigating the energy used within many steps of the brewing process.

The main brewing steps are explained here:

## Hot Liqour Tank
This is where the incomming water (either direct from the incomming water or via the heat exchanger after the boiling process in the copper.
Electrical elements of power rating Pelement are installed into base of the tank.

This is cylindrical tank of height h and diameter d.
It has insulation on the base, sides and top with U values of Ub, Us, Ut respectively.

## Mash Tun

Here the grain is mixed with water at approximately 75-80C. This creates the wort (which has the starches/sugars which are fermented into alcohol.
This process is done in an insulated tank, but does not require any additional energy input.

## Copper

In the copper the wort from the Mash Tun is boiled. Electrical or gas heaters on the base of the copper which raises the temperature of the wort to a rolling boil. The rolling boil is maintained for 1-2 hours and hops are added for bitterness and flavour.
A loose fitting lid may or may not be used in the process.

## Heat Exchanger

The heat exchanger is used to recover some of the heat from the hot product from the Copper. This is typically at 100-95C. Incomming cold water is used to cool the product to around 27C.
So the parameters are:
Incomming hot flow: 95C input and 27C output.
Incomming cold flow: Ambient water temperature (4-12C, depending upon season) input and 40-50C output 
Flow rates are in the region of 0.5 - 1.5 l/s.
The heat exchanger has a heat transfer coefficient of around 1000-4000 W/m2C (for flat plate exchangers).
The heat exchanger plate size depend totally upon the application. It is in the region of 3-10 m2.

The supplier of most of these heat exchanger is UK Exchangers Ltd: http://www.uk-exchangers.com/plate/

## Fermentation 

The product from the Copper is then transferred to a fermentation vessel where yeast is added and the liquid ferments into beer.
This is ideally done (for ales) at 20-22C. Heater and chillers are used to maintain the ideal fermentation temperature.

## Conditioning

The fermented beer product is then usually crash cooled to between 4-10C. The beer can then be stored until it is ready to be casked or bottled.

## Storage

The product is stored at a temperature less than 10C until it is required.

# Modelling Notes

The Hot Liquor Tank and the Heat Exchanger have been modelled using Finite Element analysis to investigate the heat transfer properties.

This has been performed using the open source program FreeFem, www.freefem.org.
The windows version can be downloaded from this link: http://www.freefem.org/ff++/windows.php
As of 2/5/2018, only the 32-bit version was stable and working. YMMV.

This needs to be installed and then the simulation scripts within this repository are used to investigate these elements.

# Details and Contact

This tool has been developed as part of the MASS- Modelling and Analytics for a Sustainable Society, through the University of Nottingham:
https://www.nottingham.ac.uk/mathematics/prospective/research/mass/mass.aspx

This was developed as part of the Energy Innovation and Collaboration - Energy For Business team:
https://www.nottingham.ac.uk/research/groups/etri/innovate-and-collaborate/index.aspx

