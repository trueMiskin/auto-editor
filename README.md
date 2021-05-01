**Auto-Editor** without opencv dependency.

**Auto-Editor** is a command line application for automatically **editing video and audio** by analyzing where sections are silent and cutting them up.

Before doing the real editing, you first cut out the "dead space" which is typically just silence. This is typically known as a "first pass". Cutting all these dead spaces is a boring task, especially if the video is 15 minutes, 30 minutes, or even an hour long.

Luckily, this can be automated with software. [Once you'll installed auto-editor](https://github.com/WyattBlue/auto-editor/blob/master/articles/installing.md), you can run:

```
auto-editor path/to/your/video.mp4
```

from your console and it will generate a **brand new video** with all the silent sections cut off. Generating a new video **takes a while** so instead, you can export the new video to your editor directly. For example, running:

```
auto-editor example.mp4 --export_to_premiere
```

Will create an XML file that can be imported to Adobe Premiere Pro. This is **much much faster** than generating a new video (takes usually seconds). DaVinici Resolve and Final Cut Pro are also supported.

```
auto-editor example.mp4 --export_to_resolve
```

```
auto-editor example.mp4 --export_to_final_cut_pro
```


You can change the **pace** of a video by changing by including frames that are silent but are next to loud parts. A frame margin of 8 will add up to 8 frames before and 8 frames after the loud part.

```
auto-editor example.mp4 --frame_margin 8
```

<h3 align="center">Auto-Editor is available on all platforms</h3>
<p align="center"><img src="https://raw.githubusercontent.com/WyattBlue/auto-editor/master/articles/imgs/cross_platform.png" width="500" title="Windows, MacOs, and Linux"></p>


## Articles
 - [How to Install Auto-Editor](https://github.com/WyattBlue/auto-editor/blob/master/articles/installing.md)
 - [How to Edit Videos With Auto-Editor](https://github.com/WyattBlue/auto-editor/blob/master/articles/editing.md)
 - [How to Use Motion Detection in Auto-Editor](https://github.com/WyattBlue/auto-editor/blob/master/articles/motionDetection.md)
 - [`--cut_out`, `--ignore`, and Range Syntax](https://github.com/WyattBlue/auto-editor/blob/master/articles/rangeSyntax.md)
 - [Zooming](https://github.com/WyattBlue/auto-editor/blob/master/articles/zooming.md)
 - [The Rectangle Effect](https://github.com/WyattBlue/auto-editor/blob/master/articles/rectangleEffect.md)
 - [Subcommands](https://github.com/WyattBlue/auto-editor/blob/master/articles/subcommands.md)
 - [Branding Guide](https://github.com/WyattBlue/auto-editor/blob/master/articles/branding.md)

## Copyright
Auto-Editor is under the [Public Domain](https://github.com/WyattBlue/auto-editor/blob/master/LICENSE) but contains non-free elements. See [this page](https://github.com/WyattBlue/auto-editor/blob/master/articles/legalinfo.md) for more info.

## Donate
Bitcoin (BTC)
`bc1qpf8xufyu9klawpy3eyxenn67tedahwpvsu8uyk`

Bitcoin Cash (BCH)
`qzdw2lg7llcyx5ergjv29e9d98kl89dsm5l47kklr0`

Monero (XMR)
`4At2qRKPnksfmmJG7QdJSwBsarrFiqMrgBjJbvkohaSLXSPzjYR3jCG4wueJxs2xfoBaEVyCToL8phRkCppTiNsJ55ETyZJ`

Pirate Chain (ARRR)
`zs19e04x5x52nfrj9yxy8s67zwxl6rn3hxyzz3jem0t5dpvc9d7tnjcqr6ltjpupquw2dykksnculm`


## Issues
If you have a bug or a code suggestion, you can [create a new issue](https://github.com/WyattBlue/auto-editor/issues/new) here. If you'll like to discuss this project, suggest new features, or chat with other users, you can use [the discord server](https://discord.com/invite/kMHAWJJ).
