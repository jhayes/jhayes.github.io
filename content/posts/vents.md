+++
title = "Venting"
author = ["Jack"]
lastmod = 2024-07-01T23:34:40+01:00
tags = ["house"]
draft = false
+++

## Summary {#summary}

Clickbait title, couldn't resist the obvious one! This page is just a collection of details on the vents in my house for future Jack.


## System {#system}

There are three vents in the house with differing features.
These are then attached to an exhaust fan in the attic via ducts.
The exhaust fan is then connected to the outside via an external vent.


## Vents (Exhaust Units) {#vents--exhaust-units}

Exhaust units are the devices that pull air out of a room, also called vents.
There are three vents in the house. These are located in the kitchen, downstairs toilet and upstairs bathroom.

They all look similar but are actually different variants, all designed by Aereco.
There is a comparison table located [here](https://www.aereco.ie/products/exhaust-units-ie/bxc-2/#characteristics).

Just in case it disappears later, the gist of it is:

-   The bathroom ones have a boost feature when a person is present.
-   The kitchen and bathroom check for humidity (I guess the thinking is that a downstairs toilet won't have much water vapour anyways).
-   The kitchen one needs to be reset after the powerdown event.
-   The kitchen one's presence sensor lights up green, unlike the others (as a way of communicating diagnostics, whereas the sensor is used in the other variants and doesn't light up).

| Location          | Type      | Part Number | Humidity Sensitive | Boost Airflow | Boost Airflow based on presence detection |
|-------------------|-----------|-------------|--------------------|---------------|-------------------------------------------|
| Kitchen           | BXC^2 hps | BXC1898     | Y                  | N             | N                                         |
| Upstairs Bathroom | BXC^2 hpd | BXC1908     | Y                  | Y             | Y                                         |
| Downstairs Toilet | BXC^2 pd  | BXC1905     | N                  | Y             | Y                                         |

-   Troubleshooting guide for the [BXC^2 hps model](/vents/bxchps-beeping-troubleshooting-noise.pdf) (about the beeping).


## Exhaust Fan {#exhaust-fan}

The exhaust fan is made by Aereco also, a [V4A336](https://www.aereco.ie/products/exhaust-fans-ie/v4a-premium/) (The V4A Premium for 230V).
Looking over the manual, it's suggested that the propeller is cleaned once a year (see pg7 of the installation guide).

-   [Installation Guide](/vents/TF4496_E_V4Apremium_display-4.pdf)
-   [Product Booklet](/vents/FLY337GB_v4_display-4.pdf)
-   [Replacement Kit Booklet](/vents/TF4540_C_display-1.pdf)


## Future Stuff {#future-stuff}

-   There's a way to measure pressure using a manometer over these vents I believe, so that might be interesting to try in the future.

-   I think these vents might also have features for Co2 but I'm not sure yet.
-   The vent doors are adjustable I believe, so you can increase the amount of venting.
    -   (This could be a trade-off of heat loss vs stagnant air I think, not explored yet).
-   I haven't yet traced all the ducts around the place (starting with the exhaust).
-   The vent over the hob goes directly to an external wall for venting, not using the exhaust fan in the attic (I'm pretty sure).
