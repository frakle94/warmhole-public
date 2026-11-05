# Warmhole

Control an **A\*\*Z\*\*e** zoned HVAC system from your phone, at home and away, without paying for the manufacturer's cloud plan.

Website: **https://warmhole.dev** ¬∑ [Get started](https://warmhole.dev/start) ¬∑ [How it works](https://warmhole.dev/technical-solution) ¬∑ [The problem](https://warmhole.dev/the-problem)

> Personal, **unofficial** project. Not affiliated with or endorsed by the manufacturer. It uses the manufacturer's
> publicly documented cloud API and may stop working at any time. It is probably not in line with the manufacturer's
> terms of use: use it at your own risk, for your own home.

<p align="center">
  <img src="docs/rooms.png" alt="Rooms: system mode and one card per room with temperature, humidity and setpoint" width="300">
  &nbsp;&nbsp;
  <img src="docs/schedules.png" alt="Schedules: weekly schedules with time, days, room and action" width="300">
</p>

## The problem

The manufacturer's cloud app lets you see your system from anywhere, but since October 2026 it only accepts commands from
your home internet connection unless you pay a yearly subscription (48 EUR/year in Italy, Spain, France and Portugal).
Away from home you can look, but you cannot change anything.

## What Warmhole does

- Switch the system on and off and change mode from anywhere.
- One card per room: temperature, humidity, setpoint, on/off.
- Weekly schedules: create, edit, enable and disable.
- Works from a phone browser, installable as a web app.

## How it works, in short

The cloud accepts commands only from your home connection, so Warmhole sends them from there: a small box (an
M5Stack Atom Lite, about 15 EUR) stays plugged in at home and relays your commands to the cloud from your own network.
You talk to the Warmhole site from anywhere, and the site talks to your box.

```
phone  ->  warmhole.dev  ->  box at home  ->  manufacturer's cloud
```

- Your cloud password never leaves the box.
- The box is flashed from the browser (Chrome or Edge, USB-C cable) at https://warmhole.dev/install, no tools needed.
- Details, limits and what is stored: [How it works](https://warmhole.dev/technical-solution) and [Privacy](https://warmhole.dev/privacy).

## Status

Free public beta. It is built and run by one person in their spare time, so expect rough edges.

- Start here: [Get started](https://warmhole.dev/start) (buy the box, install, set up, sign in).
- [Beta terms](https://warmhole.dev/terms) ¬∑ [Privacy](https://warmhole.dev/privacy)
- Questions, bugs, security issues or account deletion: [Contact](https://warmhole.dev/contact).

## Common questions

**Do I need the manufacturer's paid plan?** No. That is the point of the box.

**Does it work when I am not at home?** Yes. The box is at home, you can be anywhere.

**Is it safe?** The site never asks for your cloud password, only reaches the manufacturer's cloud, and limits what the
box can be asked to do. Read the details on the [Privacy](https://warmhole.dev/privacy) page.

**Can the manufacturer block it?** Yes, at any time. It is an unofficial project.

**Is the source code available?** Not at the moment. This repository only describes the project.

