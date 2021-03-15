# Notation
On this page we will be going over the notation used throughout the document to convey the speedrun routes.

## Room notation
In this document we will be referring to rooms by their coordinates relative to the spawn room. The spawn room will always be ``(0,0)``, coordinates will be written ``(x,y)``. The x-axis will increase when traveling to the right and decrease traveling to the left, the y-axis will increase when traveling down and decrease when traveling up. This last fact may seem unintuitive but since almost all the dungeon is lower than the spawn room this will be clearer.

## Path notation
There are a few ways we will write down paths that will make writing them down a lot shorter:
- ``->``: This arrow will be used to denote walking from 1 room to one of the neighboring rooms. E.g., ``(0,0)->(1,0)`` means we walk from room ``(0,0)`` to room ``(1,0)``.
- ``=>``: This arrow will be used to denote walking several rooms over that are all in one line. E.g., ``(0,0)=>(0,3)`` is the same as writing ``(0,0)->(0,1)->(0,2)->(0,3)``.
- ``>>``: This arrow will be used to denote teleporting to a room, this game mechanic is only used in the Orb of Life dungeon. E.g., ``(0,0)>>(5,4)`` means we teleported from room ``(0,0)`` to room ``(5,4)``.
- ``=<``: This arrow will be used to denote when we return to a certain room the same way we got to the current room from there. E.g., ``(0,0)=>(5,4)->(5,5)>>(3,1)=<(0,0)`` is the same as writing ``(0,0)=>(5,4)->(5,5)>>(3,1)>>(5,5)->(5,4)=>(0,0)``.

We will also be denoting repeated screen changes since these sometimes happen (for example in Any% Golden Spider), these will be denoted with ``{(x1,y1 ).<->(x2,y2)}a`` where ``(x1,y1)`` is the room we first enter and ``a`` is the amount of times we switch room. The dot next to the arrow indicates which room we end in. If the repeated screen changes happen because of teleporters ``<->`` will be replaced with ``<<>>``. E.g., ``(2,-4)->(2,-3)->(2,-4)->(2,-3)->(2,-4)`` becomes ``{(2,-4).<->(2,3)}4``. This way of writing down screenchanges main only be used over normal notation if ``a`` is larger or equal to 3.

### Rule of Simplicity
An additional rule is that if there are multiple ways to write a path that have the same length, the simplest must be chosen. E.g., ``(4,1)->(4,0)->(3,0)=<(4,1)->(4,2)`` and ``(4,1)->(4,0)->(3,0)->(4,0)=>(4,2)`` mean the same thing but the latter is much simpler.

For this purpose we have developed a point system to make these decisions more easily:
| Arrow | Points |
|:---:|:---:|
| ``->`` and ``>>`` | 1 |
| ``=>`` | 2 |
| ``=<`` | 4 |

If multiple ways of writing the same path exist that are all the same length, the one with the lowest score must be chosen.

## Collectibles and dungeon ending
There are quite a few collectibles in this game, we will be using these symbols to denote collecting them:
- ``*``: This symbol next to a room will be used to denote essential collectibles, like diamonds in Chalice of The Gods. E.g., ``(3,4)*`` means that in the room ``(3,4)`` we collect an essential collectible.
- ``$``: This symbol will, unsurprisingly, be used to denote collecting coins. To symbolize how many coins you collect in a given room we will put a number behind the symbol. E.g., ``(4,3)$5`` means we collected 5 coins in room ``(4,3)``.
- ``♥``: This symbol will denote picking up a heart container. E.g. ``(4,3)♥`` means we picked up a heart container in room ``(4,3)``.
- ``%``: This symbol will be used to denote rooms where it is important to pick up ammo. E.g., ``(5,2)Φ`` means we picked up ammo in room ``(5,2)``.
- ``⊡``: This symbol will be used to denote picking up a scroll. E.g., ``(-1,3)⊡`` means we picked up a scroll in room ``(-1,3)``.
- ``!``: This symbol will denote the end of a dungeon. E.g., ``(5,4)!`` means room ``(5,4)`` is an ending room in a dungeon.

These symbols will only be denoted in routes where they matter and will always be in order of importance behind a room: ``(x,y)!⊡*$♥%``.

## Modifiers
For the full game runs modifiers also must be collected, this is how they will be noted:
- ``D``: Will be used to denote collecting the Double Jumps modifier.
- ``I``: Will be used to denote collecting the Infinite Ammo modifier.
- ``R``: Will be used to denote collecting the Rhino Armor modifier.

## Menuing 
In full game runs some menuing can be used, to denote this we will use the following notation:
- ``⊗``: Will denote exiting a dungeon.
- ``[a]``: Will denote selecting a dungeon, ``[1]`` for Chalice of The Gods, ``[2]`` for Golden Spider, and ``[3]`` for Orb of Life.
