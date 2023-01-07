# Mcblend Project Template

This repository contains a Blender template file for Mcblend projects. Mcblend
is a Blender 3.3 plugin that enables creators to design and animate Minecraft
Bedrock Edition models using Blender's powerful 3D modeling and animation
tools.

**Mcblend Repository**: https://github.com/Nusiq/mcblend

## Adding the Template to Blender

Instructions for adding the template to your Blender installation can be found
in the Blender documentation:
https://docs.blender.org/manual/en/latest/advanced/app_templates.html#directory-layout.

**TLDR:** Add the `startup.blend` file to the folder in
`%appdata%\Blender Foundation\Blender\3.3\scripts\startup\bl_app_templates_user\Minecraft`
(this path may be different on your computer). After that, you should be able
to use it for new projects from the `File > New > Minecraft` menu.

## Template description
### 3D Viewport

The project is set up to facilitate the creation of animations for attachable
items in Minecraft.

- The scene contains a model of a Minecraft Alex character
- The camera (`Player View`) is positioned in the same way as a Minecraft
  camera in the first-person mode
- The player armature (`humanoid.customSlim`) has a pose that moves the arms in
  a way that closely resembles their positions in the first-person mode

### Animations

The settings are configured to make it easier to create Minecraft animations.

- The frame rate is set to 25 FPS. 25 divides 1 second more evenly than the
  default 24 FPS, which is important because the timeline in Minecraft
  animations is in seconds, not frames.
- The subframes are enabled by default in playback, and snapping to the nearest
  frame when moving the frames on the timeline is disabled. This makes it
  easier to work with Minecraft animations that are not limited by frames.

### Workspaces

There are 4 workspaces in the template, each of them is set up for a different
type of work commonly performed when working with Minecraft models. The setup
is similar to the default Blender workspaces, but some of the workspaces that
are not useful for Mcblend are removed and some of the other workspaces are
modified to make them more useful for Mcblend.

- **Modeling** - a workspace with a large 3D viewport for modeling.
- **Animation** - a workspace with an NLA editor, a Dope Sheet, and a Timeline
  editor. These editors are commonly used in Mcblend because Mcblend maps
  Minecraft animations to Blender's NLA tracks.
- **UV Editing** - a workspace with a UV editor and a 3D viewport, for working
  on UV maps and textures.
- **Material Preview** - a workspace for viewing materials. Mcblend generates
  materials automatically, so this workspace is rarely used.
