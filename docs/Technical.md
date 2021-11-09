# Technical details

The patcher carries over all changes from ELE that have been reverted by another plugin coming after ELE in the load order. Only reverted changes are patched, not new ones - if the other plugin makes a change of its own, it's kept.

A change refers to the difference of a value between one of ELE's masters and ELE itself. Each master is taken into account separately. Relighting Skyrim is counted as a "master", to assure that when there's conflict between the two, ELE's change will win, as these two were meant to be used together.

Value can refer to a single field, or a bunch of grouped together fields. For example, ELE changes many things about cells' lighting: Directional colors, specular colors, fog clip distances, etc... These values relate very closely together, so they're counted as just one value changing: Lighting.

For example, in my load order, I have Immersive College of Winterhold changing a cell's Directional XY from 0 to 180, and ELE changing Directional Z from 0 to 90. Combining these two changes... No clue what that would look like, so to keep it safe, the patcher will just keep all lighting from whichever one is later in the load order.

## ELE changes

- Image spaces
  - HDR
  - Cinematic
  - Tint
- Lights
  - Record flags
  - Flags
  - Object bounds
  - Radius
  - Color
  - Near clip
  - Fade value
- Worldspaces
  - Interior lighting
- Cells
  - Lighting
  - Lighting template
  - Water height
  - Water noise texture (I don't think this does anything, they're all empty values, really just to stop xEdit complaining)
  - Sky and weather from region
  - Image space
- Placed objects
  - Record flags
  - Primitive
  - Light data
  - Bound half extents
  - Unknown
  - Lighting template
  - Image space
  - Location reference
  - Placement

# Another yes.

- Image Spaces: HDR, cinematic, tint
- Lights: record flags, flags, object bounds, radius, color, near clip, fade value
- Worldspaces: interior lighting
- Cells: lighting, lighting template, water height, water noise texture, sky and weather from region, image space
- Placed objects: record flags, primitive, light data, bound half extents, unknown, lighting template, image space, location reference, placement