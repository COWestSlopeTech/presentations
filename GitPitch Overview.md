## Overview

GitPitch provides a simple, free, version controlled presentation facility that is readily viewable from any computer connected to the internet. It is becoming a programming presentation standard at recent conferences.

Pros:

* Presentation is a text document - no proprietary, OS specific, paid software required. Anyone can generate or collaborate on presentations.
* Our organization, one presentation per directory, allows simple storage and access to all assets
* Audience has access to the presentation and all assets before, during, and after the presentation

Cons:

* Doesn't have the visual point and click simplicity of KeyNote or PowerPoint.
* Doesn't have the rich theming available in KeyNote or PowerPoint.
* Developing the pitch can be tedious without the Desktop App

## References

* [Features](https://gitpitch.com/features)
* [Docs](https://gitpitch.com/docs)
* [Template Gallery](https://gitpitch.com/templates)
* [Kitchen Sink](https://gitpitch.com/gitpitch/kitchen-sink#/)


## Create a new presentation

Each presentation resides in its own directory, in a single `PITCHME.md` and configured by a `PITCHME.yaml`.

1. Create a new directory with a name that indicates the presentation.
1. Add a `PITCHME.md`, `PITCHME.yaml`
1. Create a `README.md` that will contain general notes for offline viewing or using the assets
1. Create a `pitch` directory that will contain all pitch assets - images, etc.


## Iteratively develop the presentation

**NOTE**: If you use GitPitch frequently, the Desktop App is included in the Lite version ($4/mo) and should trivialize much of this work.

To shorten the write-push-view loop:

1. Create a skeleton one-page presentation and git-push it.
1. Open your skeleton one-page presentation on gitpitch.com.
1. Click the burger-menu and then "Offline Version" to download the self-contained presentation bundle.
1. Follow instructions from [here](https://gitpitch.com/docs/foundation-features/offline/) to run the presentation. E.g.
    1. Copy the `PITCHME.zip` file to your project directory and expand it, creating a `PITCHME` directory.
    1. `cd PITCHME`
    1. `python3 -m http.server`
    1. Edit the pitch at `assets/md/PITCHME.md`
    1. Reload the pitch after edit to view the results.
1. When edits are complete, merge the above into your main PITCHME.md

### Domain markdown

https://gitpitch.com/docs/markdown-features/shortcuts/

### Background images

The slide delimiter (`---`, `+++`) marks the beginning of a slide. Add an image to that and it becomes the background image.

```
---?image=svgo/pitch/images/gopherhat.jpg
```
Not the similarity to a url query string.

The path is relative to the repo root - don't forget the sub-directory if you are using a single repository for multiple presentations.

* SVG images require purchasing the 'pro' package.


### Add an image to a slide

### Formatting

