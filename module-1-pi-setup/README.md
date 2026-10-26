# Module 1: Raspberry Pi Setup

## Overview
In this module I set up a Raspberry Pi as my lab environment for CS-350. The goal was to get the Pi running, connected to my home network, and reachable from my laptop over SSH so I could work on it remotely.

## What I did
- Set up the Pi with Ubuntu 24.04
- Configured Wi-Fi using netplan (this version of Ubuntu doesn't use nmcli)
- Set the hostname to cs350lab so I can reach it at cs350lab.local
- Connected from my laptop over SSH

## Problem I ran into
After switching internet providers, my Pi's IP address changed because the new router assigns addresses automatically. I had to find the new address before I could connect again. Using the hostname instead of the IP makes this easier.

## What I learned
Network settings can change without warning, so it helps to know how to track down the new address instead of assuming the old one still works.

## Screenshots
(Add screenshots here with a sentence explaining each one.)
