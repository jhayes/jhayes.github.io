+++
title = "Venting"
author = ["Jack"]
lastmod = 2024-06-28T09:58:16+01:00
tags = ["house"]
draft = false
+++

## Summary {#summary}

Clickbait title, couldn't resist the obvious one! This page is just a collection of details on the vents in my house for future Jack.


## Details {#details}

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


## Future Stuff {#future-stuff}

-   There's a way to measure pressure using a manometer over these vents I believe, so that might be interesting to try in the future.
-   I think the vents all make their way up to the attic, where there's a much larger exhuast, but I'm not completely sure on that yet.
    -   At the same time, we also have a vent over the hob but that's venting a different way I think.
-   I think these vents might also have features for Co2 but I'm not sure yet.
-   The vent doors are adjustable I believe, so you can increase the amount of venting.
    -   (This could be a trade-off of heat loss vs stagnant air I think, not explored yet).


## Links {#links}

-   This is a troubleshooting guide for the [BXC^2 hps model](/bxchps-beeping-troubleshooting-noise.pdf) (about the beeping).
