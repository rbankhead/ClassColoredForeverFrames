# ClassColoredForeverFrames

A World of Warcraft: Forever addon that colors your player frame's health bar by your class, and your target frame's health bar by their class when your target is a player (otherwise the normal reaction color).

## Installation

Drop the `ClassColoredForeverFrames` folder into your `Interface/AddOns` directory.

## How it works

The player/target health bars are nested four levels deep in the default UI and both lock their own color, so nothing else recolors them once set. Their bar texture has a styled gradient baked in rather than being a neutral white bar, so a plain color tint would come out muddy - the texture is desaturated first to strip its baked-in hue while keeping its real shape and shading, so the class/reaction color tint reads correctly without changing the bar's look.

## Requirements

WoW: Forever (Interface 16001).
