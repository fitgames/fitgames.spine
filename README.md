# FitGames.Spine 
<img src="https://ci.appveyor.com/api/projects/status/nfat1fqjtg9cqc4v" alt="build status" >

FitGames.Spine is an extension of the <a href="https://github.com/EsotericSoftware/spine-runtimes/">Spine Runtime</a>, and the XNA supporting objects.

### Other Modifications

There is a new namespace added with two objects `ContentAtlas` and `ContentSkeletonJson` which inherit from `SkeletonJson`. These were created to load Spine objects from the content of the files instead of using a Stream or relying on XNATextureLoader.

The second, perhaps more important is because they are used in our MonoGame pipeline extension which allows zipping atlas.txt, skeleton.json, and skeleton.png into a zip file. This new zip file can be process by the pipeline and loaded using `Content.Load<SpineAsset>('assetkey')` with ease, and ready for rendering.


