---
title: "Connecting Unreal Engine's Lyra and UltraDynamicSky Sound"
date: 2022-08-02T23:11:30-04:00
categories:
  - Audio
  - Sound
tags:
  - UltraDynamicSky
  - UE5_Lyra

gallery:
 - url: /assets/images/Posts/AudioGraph_LyraUDS.png
   image_path: /assets/images/Posts/AudioGraph_LyraUDS.png
   alt: "Lyra Audio Graph with UDS"
   title: "Lyra Sound Class with UltraDynamicSky"
---

# Connecting Unreal Engine's Lyra and UltraDynamicSky Sound


This is a simple setup to connect `Unreal Engine's Lyra` **Sound** Settings Menu with `UltraDynamicSky`'s Sound for Weather.

1. Open up your Sound Class `Main` under `/Game/Audio/Classes/Overall`. This will open up a graph That looks similar to the below image.
1. You'll need to drag and drop your UltraDynamicSky (UDS) Sound classes here to create a reference to them.
    1. Alternatively, click the Class you want to make them children of, I recommend the SFX Class. and add them to the `Child Classes` field under details.
1. Last thing is to select each of the new child nodes, and under the **Details** panel, Modulation, Enable Volume Modulation, and set the class to be `PP_DefaultSFX`. 

{% include gallery %}


![LyraAudioGraph_UDS](/assets/images/Posts/AudioGraph_LyraUDS.png)