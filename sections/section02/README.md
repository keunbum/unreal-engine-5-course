# Section2: Realistic Landscapes


## Table of Contents

1. [Quixel Bridge](#quixel-bridge)
2. [Open World](#open-world)
3. [Lighting and Atmosphere](#lighting-and-atmosphere)
4. [Landscape](#landscape)
5. [Landscape Material](#landscape-material)
6. [Landscape Painting](#landscape-painting)
7. [Foliage Painting](#foliage-painting)
8. [More Foliage Painting](#more-foliage-painting)
9. [Post Process Volume](#post-process-volume)
10. [Forest Polish Up](#forest-polish-up)
11. [Packed Level Actors](#packed-level-actors)
12. [Mountains](#mountains)
13. [Level Instances](#level-instances)
14. [Section 2 Challenge](#section-2-challenge)

---

### Quixel Bridge

Learn how to download and deploy Assets from Quixel Bridge.

[Quixel Bridge for UE5](https://help.quixel.com/hc/en-us/articles/360020717197-How-do-I-open-Quixel-Bridge-in-the-Editor-)

### Open World

[Open World Tools](https://docs.unrealengine.com/5.1/en-US/open-world-tools-in-unreal-engine/)

#### Large Worlds

Typically, a large world is broken up into multiple levels.

Now, this is a lot of work to set up and to manage,  
but Unreal Engine 5 has introduced a workflow that makes this much easier.  
Unreal Engines Open World system allows us to have one map instead of multiple.  

So instead of several small maps, we have one single large map  
and Unreal Engine is in charge of splitting this world up into sections  
and only loading that section that our player is in.

This is called World Partitioning and we don't have to set up multiple maps and manually load and unload
them as the player walks around through the world.


### Lighting and Atmosphere

[Landscape Quick Start Guide](https://docs.unrealengine.com/5.1/en-US/landscape-quick-start-guide-in-unreal-engine/)

* Sky Atmosphere
    * Creates an earth like atmosphere
    * Scatters light just like a real atmosphere
    * Can have up to two atmosphere lights

* Directional Light
    * light source infinitely far away
    * Shadows cast from it are all parallel
    * Simulates the sum (or moon)

    * Mobility
        * Static
            * Lighting cannot be changed in-game
            * Fastest
            * Allows baked lighting
        * Stationary
            * Color and Intensity can change in-game
            * Allows partialy-baked lighting
        * Movable
            * Can be moved and changed in-game
            * Dynamic shadows

* Sky Light
    * Captures distant parts of the level
    * Applies to the scene as light (reflections)
    * Global illumination
    * **Captures** only in certain conditions:
        * For static lights, updates when building lighting
        * For stationary and movable lights, updates once on load and on **Capture**
        * Constantly when Real-Time Capture is enabled

* Exponential Height Fog
    * Simulates Fog
    * Gets thicker the lower you go
    * Two colors
        * Hemisphere of a planet facing the sun
        * The other hemisphere

* Volumetric Clouds
    * Dynamic Clouds
    * 3-dimensional
    * Material driven
    * Light-scattering


### Landscape


### Landscape Material


### Landscape Painting


### Foliage Painting


### More Foliage Painting


### Post Process Volume


### Forest Polish Up


### Packed Level Actors


### Mountains


### Level Instances


### Section 2 Challenge