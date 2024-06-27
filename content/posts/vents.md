+++
title = "Vents"
author = ["Jack"]
lastmod = 2024-06-27T23:41:15+01:00
tags = ["house"]
draft = true
+++

## Introduction {#introduction}

There are three vents in the house. These are located in the kitchen, downstairs toilet and upstairs bathroom.

They all look similar but are actually different variants, all designed by Aereco.
There is a comparison table located here: <https://www.aereco.ie/products/exhaust-units-ie/bxc-2/#characteristics>

Just in case it disappears later, the gist is:

-   The bathroom ones have a boost feature when a person is present.
-   The kitchen and bathroom check for humidity (I guess the downstairs toilet won't have much water vapour anyways).
-   The kitchen one needs to be reset after the powerdown event.
-   The kitchen one's presence sensor lights up green, unlike the others (as a way of communicating diagnostics, whereas the sensor is used in the other variants).

| Location          | Type      | Part Number | Humidity Sensitive | Boost Airflow | Boost Airflow based on presence detection |
|-------------------|-----------|-------------|--------------------|---------------|-------------------------------------------|
| Kitchen           | BXC^2 hps | BXC1898     | Y                  | N             | N                                         |
| Upstairs Bathroom | BXC^2 hpd | BXC1908     | Y                  | Y             | Y                                         |
| Downstairs Toilet | BXC^2 pd  | BXC1905     | N                  | Y             | Y                                         |


## Other Details {#other-details}

-   There's a way to measure pressure using a manometer over these vents I believe, so that might be interesting to try in the future.
-   I think the vents all make their way up to the attic, where there's a much larger exhuast, but I'm not completely sure on that yet.
    -   At the same time, we also have a vent over the hob but that's venting a different way I think.
-   I think these vents might also have features for Co2 but I'm not sure yet.
