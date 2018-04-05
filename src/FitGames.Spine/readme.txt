#FitGames.Spine

Spine Runtime with support for MonoGame, and two new Pipeline objects to support MonoGame pipeline extensions.

#Changes

The latest Spine Runtime removed SkeletonMeshRenderer in favor of using SkeletonRenderer moving forward. In our case we
kept both to avoid rushing the transition. The main reason has to do with SkeletonRenderer needing an effect file to work.

https://github.com/EsotericSoftware/spine-runtimes/blob/3.6/spine-xna/example-content/SpineEffect.fx

