---
title: "Cobalt+ Guides: Multibay"
permalink: /c+guides/multibay
parent: Cobalt+ Guides
---

### Welcome!

**This guide will walk you through setting up a Multibay System (where 2 or more lifts are linked using the same call buttons) using Cobalt+.**<br>
You require some proficiency in using Roblox Studio.

#### Table of Contents
- TOC
{:toc}

### Video
This video guide will walk you through all the steps below in a video format.
<iframe width="560" height="315" src="https://www.youtube.com/embed/HlkJduZ3Icg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Guide
### Things you'll need:
- 2 or more lifts
- [Pre-setup Multibay](https://create.roblox.com/store/asset/12783114215)

### Step 1: Setup
To start, insert the Multibay setup from the toolbox into your game, this provides the foundation to setup the Multibay system.

{: .highlight }
> You can do either Step 2a or 2b first, it doesn't matter.

### Step 2a (easier to do this first)
Drag the call buttons out of your lift (UpCall, DownCall), these are located in every single floor within Shaft.

Parent them to Workspace or whatever you're comfortable with.

### Step 2b: Lifts
Next, drag your lift models into the "Lift" section of the Multibay Setup (Multibay > Lifts).

Make sure to rename your lifts to something like "A" and "B". Lift names **cannot** start with numbers.

### Step 3: Call Buttons
Drag your **call buttons** (UpCall, DownCall) into their corresponding floor (e.g. Floor 1 Call buttons go into Floors>1) within the "Floors" section of the Multibay. Create more Floors as needed (1,2,3 etc.).

{: .warning }
> Rename the call buttons to **Up** and **Down**, they will **NOT** work without this renaming.

### Step 4: Configuration
At this point you can open your Multibay configuration file.<br>
It should look like this:
```lua
--Multibay Config

return {
	--/ Button /--
	["ClickDetector"] = false, -- Apply Legacy ClickDetector, but not for Alarm button
	--["CallLock"] = {}, -- Locked Call Buttons
	["ButtonLit"] = "Bright blue", -- Default Button Lit Colour
	["ButtonUnLit"] = "Institutional white", -- Default Button UnLit Colour
	
}
```

You can change the color of the Call Button lighting here.
You can copy it over from the Script file of your lift, it has the same name. For example:
```lua
["ButtonLit"] = "Neon orange", -- Default Button Lit Colour
["ButtonUnLit"] = "Medium stone grey", -- Default Button UnLit Colour
```

If you'd like to lock any floors, simply add them to "CallLock", same as you would for regular lift configuration. Remember to remove the comment (--) at the start of the line.
Example:
```lua
["CallLock"] = {1,2,3}, -- Locked Call Buttons
```

That's it!
Your Multibay is now setup and ready to go.
These are the only things you need to do!

---
### Thanks for reading!
I hope this guide has been helpful to you. <br>
All my resources are provide for free, feel free to check out the other guides on this page!

If you'd like to hang out with a fun community, do join our Discord Server linked down below.

### Contact and Connect:
Discord: @matt_wyz<br>
YouTube: [@matsq4](https://youtube.com/@matsq4)<br>
Instagram: [@matsq4](https://instagram.com/matsq4)<br>
Ko-fi: [@matsq4](https://ko-fi.com/matsq4)

matsq4 Group DISCORD Server: [discord.gg/BKMzZZU4Vg](https://discord.gg/BKMzZZU4Vg)<br>
matsq4 Group WEB: [matsq4group.com](https://www.matsq4group.com)
