# freeswitch-mod
Repository collecting various freeswitch modules that needs to be compiled with wgtwo freeswitch deployment

## Purpose

This repository is meant to be copied to the root of https://github.com/signalwire/freeswitch
before building in order to compile the modules in this repo together with freeswitch compilation.

This is needed for some wgtwo Freeswitch deployments, like voicemail for Norwegian userbase.

The folder structure of this repo is similar to the folder structure of [`Freeswitch`](https://github.com/signalwire/freeswitch) code and is meant to just be copied into the root folder of [`Freeswitch`](https://github.com/signalwire/freeswitch)

## How to use this repo

This repo is meant to be cloned before building freeswitch docker image.
The files in this repo are in the same folder structure as [`Freeswitch`](https://github.com/signalwire/freeswitch).

The `configure.ac` file in this repose is taken from the official repo for the current version we are working on: `v.1.10.8` and the only line added to it is the following line: `src/mod/say/mod_say_nb/Makefile`, which makes the Norwegian say module discoverable to `Freeswitch` build system.