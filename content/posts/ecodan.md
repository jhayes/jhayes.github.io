+++
title = "What I know about Ecodan ASHPs"
author = ["Jack"]
date = 2024-06-18T00:00:00+01:00
lastmod = 2024-07-01T22:59:56+01:00
tags = ["house", "heating"]
draft = false
+++

## Summary {#summary}

The following is a meandering post on what I've learnt about heat pumps (and more specifically the Ecodan range from Mistubishi) and some handy resources I've found.


## The System {#the-system}

The gist of the sytem is shown in the following infographic.

{{< figure src="/heatpumps/infographic.jpeg" link="/heatpumps/infographic.jpeg" >}}


### The Outdoor Unit {#the-outdoor-unit}

I'm using an 5kW Mitsubishi Ecodan Air to Water Heat Pump. It uses [R32](https://en.wikipedia.org/wiki/Difluoromethane) as its refrigerant.
It's a **Monobloc** unit, this means that the refrigerant is all contained outdoors and only water migrates into the house.

There are two sides to every heat pump, the source and the sink. One can think of the source (air passing through the fan outdoors) as the input and the sink as the output (our radiators, etc).
In this case, our source is Air and our sink is Water.

-   [Ecodan PUZ-WM50VHA Information Sheet](/heatpumps/Ecodan_PUZ-WM50VHA_Monobloc_Air_Source_Heat_Pump_Product_Information_Sheet.pdf)
-   [Ecodan PUZ-WM Installation Guide](/heatpumps/EcodanPUZ-WM_50-60-85-112_V_H-A_A_Installation_Manual__BH79D849H02UK_.pdf)
-   [Ecodan PUZ-WV50VHA (OCH727) Service Manual](/heatpumps/Ecodan_PUZ-WM_50-60-85-112_V_H-A_A_Service_Manual__OCH727A_.pdf)


### The Indoor Unit (Cylinder Unit) {#the-indoor-unit--cylinder-unit}

Judging by the label on the unit, this an EHPT17X-VM2DR1.UK model. The 17 in the title means that it has a 170 litre DHW (Domestic Hot Water) tank.

-   [Ecodan EHPT17X-VM2DR1.UK Service Manual](/heatpumps/Ecodan_EHPT20X-MHEDWR1_Service_Manual__OCH714E_.pdf)


### The Controller {#the-controller}

This system uses the FTC6 controller. From our point of view, this consists of a collection of dip switches for initial setup and then an LCD display for modifying on the go.

-   [Ecodan FTC6 Instruction Book](/heatpumps/Ecodan_FTC6_PAC-IF07_1-3_B-E_Instruction_Book__BT79R180H01_.pdf)
-   [Handy video](https://www.youtube.com/watch?v=0Y4w18656d0) explaining the dip switches on the FTC6.
    -   Covers some of the points on two zone systems.


### Map of the Plumbing {#map-of-the-plumbing}

The following image is a map of the pipework above the cylinder unit, with labels.
Some of this is based off the labels attached to the pipes and other parts are guesswork.


#### DHW Details {#dhw-details}

-   There are two feeds of water coming in.
    -   One of these is labelled cold; I think this comes from the tank in the attic.
        -   (It could be coming from mains but I don't think it is because it's coming down from the ceiling so seems like an unlikely path).
    -   The other one is labelled hot. I think this is a return path from the hot water that orginates from the cylinder unit.
-   These mix together and go into the heat pump.
    -   There is also a header tank here and an overflow.
-   These then come back out and go out again towards all three of the hot water taps and the shower.

{{< figure src="/heatpump_map_1.jpeg" link="/heatpumps/heatpump_map_1.jpeg" >}}


#### Radiator Details {#radiator-details}

-   Starting from the left, I think these are two return paths for the radiators.
-   They combine together and then enter a filter before going into the unit.
    -   (The filter is a [Fernox TF1 Sigma Filter](https://fernox.com/product/tf1-sigma-filter/), which has a 10 year warranty).
    -   [TF1 Sigma Filter 28mm Data Sheet](/heatpumps/62417-TF1-Sigma-Filter.pdf)
        -   This data sheet shows how to clean the filter also.
-   The heated up fluid then comes out of the cylinder unit, from the second pipe from the left.
    -   There are two tap points here with a valve between.
        -   I think this is to allow for an underfloor heating loop to be added on conveniently.
    -   This hot line then goes up and branches into two separate lines.
    -   Each line has a motorized control valve on it.
        -   (Adjusting the thermostats in the rooms seems to have an effect on these, lighting them up).
        -   [EPH V222PW Installation &amp; Technical Spec Document](/heatpumps/2023-04-27_V22_P-FP_DS_PK_Email.pdf)


#### Other Details {#other-details}


## Adding a smart sensor {#adding-a-smart-sensor}

It's possible to add a smart sensor to this heating system. The model number I used was 587IF-E.

When I was trying to source this, there was confusion online about the fact that there are multiple variants.
It seems like there's a different part number for Austrialian models (or something).

I bought mine on [eBay](https://www.ebay.ie/itm/284060037125) and it seemed to work fine.

For installation, I used the following videos:

-   <https://www.youtube.com/watch?v=XZj4t4kwYVQ>
-   <https://www.youtube.com/watch?v=i1wABPBAWK8>

{{< figure src="/heatpump_sensor_1.png" link="/heatpumps/heatpump_sensor_1.png" >}}


## Diagnostics {#diagnostics}


### Pressure Gauge {#pressure-gauge}

-   Previously I had a slight weep in the system. There's a gauge that indicates the pressure of the system.
-   From talking to the plumber and heat pump service guy, keeping it in the range of 1 to 2 bar is what you're looking for, they advise.

{{< figure src="/heatpump_gauge_28jun24_1.jpeg" link="/heatpumps/heatpump_gauge_28jun24_1.jpeg" >}}

{{< figure src="/heatpump_gauge_28jun24_2.jpeg" link="/heatpumps/heatpump_gauge_28jun24_2.jpeg" >}}


## Links {#links}

-   The book [Heat Pumps for the Home](https://www.amazon.co.uk/Heat-Pumps-Home-John-Cantor/dp/1785007793/ref=sr_1_3?crid=14CXTV81MAL5A&dib=eyJ2IjoiMSJ9.v79c5G2CcnKI1ma3zMB0zVfWk5pPPkDXTLfbsC-64gLOs0P7-k5QmsNHMl6MvnMme-zdApiBmqPOIBYYy1njTr-ooDyW2xDh2LObpWiuChLoh3gfUWpgvm9RRgTBqqgLw94QgnSSTsMZa9DYmIlriGowM4sAgE5DqFHesfkOyMCkcw0z1vzvn7H0Omk-lEDT7lJ9Zan8qhScqMGUCUnn3gLC_L5l8WvdtLHKgKVvkpA.BLOOjOyIAwjk3ynCdH0Zj3D8ZMmsLSbQhqrCL1Z7tYQ&dib_tag=se&keywords=heat+pumps+for+the+home&qid=1719574691&sprefix=heat+pumps+for+the+%2Caps%2C72&sr=8-3) was pretty good.
    -   It actually includes a lot of systems that use Ecodans.
