# Validation

Store hand calculations and test cases in this folder.

## Implemented regression cases

Open the app through a local HTTP server and use the browser console to verify:

```text
BeamDesignerResult.reactions
```

The baseline example is a 20 ft simply supported beam with a full-span uniform
load of 1 kip/ft and the W12x26 section:

- Maximum moment: 50.0 kip-ft
- Maximum deflection: approximately 0.609 in
- Reactions: 10 kip at each support
- Deflection limit: 20 ft / 360 = 0.667 in

Run additional cases for:

- Center point load on a simply supported beam
- End point load on a cantilever
- Full-span uniform load on a cantilever
- Multiple point loads
- Mixed point and uniform loads
- Lumber edgewise and flatwise orientations
