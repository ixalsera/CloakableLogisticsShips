# Cloakable Logistics Ships

A Stellaris mod that lets Nomadic empires cloak their Logistics Ships, letting them harvest deposits from other empires' systems with the same modifier as cloaked waystations.

## Overview

In vanilla, when you issue the Harvest Resources action to a Logistics Ship for a system owned by another empire, every resource that gets harvested applies a -75 penalty to the opinion of that empire, capping at -1000. If a system has 7 objects that are harvestable, that's -525 opinion in one go. Got four Logistics Ships on auto? Say goodbye to your opinion with that empire!

Waystations can be equipped with cloaking technology that reduces the penalty by 50%, so why not have the same feature for Logistics Ships too? After all, why cloak the station when the empires can just watch your ships vanish in to thin void when collecting from them to work out where they are?!

Added benefits? Logistics ships can now pass through hostile space to return your precious operation reserves resources to you instead of just chilling waiting for that space amoeba to die of old age. Or go harvest from Papqaqvet 
## Features

- **New cloaking utility slot** on the Logistics Ship (and Logistics Vessel for Eager Explorers!) that functions the same as vanilla Science Vessels (auto-upgrades, shield nullification, sub-light penalties).
- **New fleet actions** - "Activate Cloak" and "Deactivate Cloak", added to the Logistics Ships' fleet view actions panel with a 120-day cooldown.
- **Halved opinion penalty** - harvesting a deposit while cloaked applies a new "Sneakily Harvested Resources" opinion modifier, mechanically identical to the vanilla penalty but at -50%.

## Requirements

- Stellaris 4.4 or later
- Nomads DLC (for logistics ships, duh)
- First Contact DLC (for cloaking tech)

## Compatibility

This mod patches the following vanilla files, so it may conflict with other mods that touch the same things:

- The `nomads_constructor` and `nomads_engineer_vessel` ship sizes (adds the cloaking component set and the two fleet actions)
- The `nomads.4100` event fired by `on_harvest_resources` (checks the harvesting ship's cloak state to pick the right opinion modifier)

## Installation

Subscribe on the Steam Workshop, or copy this folder into your Stellaris `mod` directory and enable it from the in-game mod launcher.

## Known Issues

- Cloaking is a full fleet action. I can't find any way to make it a state toggle like for other vessels. This means it _*WILL*_ cancel your current fleet order(s) unless you queue it.
- Decloak button doesn't show the time remaining on the cooldown. It's a minor thing and if I find a way to fix it I will, but otherwise it's not stopping anything.
