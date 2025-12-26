# BloonsTD

Bloons-TD is a tower defense game made in Unity2d and programmed in C#. It is a simplified adaptation from the BloonsTD series. The goal of this game is to defeat hordes of bloons using monkeys and prevent bloons from destroying your home base.

The challenges in this game was that I had to use 3 different monkey types to defend against 3 different bloons. Defeating bloons grants the player currency which can be spent to add additional monkeys and bolster defenses. The basic monkey shoots at a slow rate and costs the least. The ninja monkey shoots at a higher rate and costs more than the basic. The sniper monkey shoots at the highest rate and can pop metal bloons but costs the most too. The red bloon moves at a fast pace but can be popped easily. The blue bloon moves slower and can be popped easily but on popped, it releases more red bloons. The metal bloon is the slowest but can only be popped by the sniper monkey but also released multiple blue bloons once popped which in turn releases multiple red bloons, the screen can get overwhelmed if resources for defense are not spent wisely.

Coding all of this is very complicated, resource taxing and inefficient, hence I have decided to use singletons. Singletons ensure that classes only have one instance and provides global access to it. Implementing singleton for monkey shooting, bloon spawning and popping has removed lots of redudant code from the project and improved overall efficiency. Using generic singletons can further improve upon this.

We have many waves where the frequency of these bloons differ. But creating all of these dependencies again whenever the wave is loaded can be CPU intensive. Therefore, I have used dependency injections. It is design pattern where an object receives its dependencies, i.e., other objects it needs from an external source rather than creating them itself, promoting loose coupling, testability, and modularity by "injecting" them, often via a constructor, which makes code easier to manage and reuse.

Demo video:

