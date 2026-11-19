# Data

Store project data files in this folder.

`beam_sections.json` is the built-in section-property database used by the
Beam Designer MVP.

- Steel records contain `designation`, area, depth, weight, strong-axis \(I_x\),
  strong-axis \(S_x\), modulus \(E\), and allowable bending stress \(F_b\).
- Lumber records contain nominal and actual dimensions, species, grade,
  edgewise or flatwise orientation, strong-axis \(I\), strong-axis \(S\),
  modulus \(E\), and base bending stress \(F_b\).
- The JSON `sources` metadata identifies the property-table basis and its
  revision caveats.

The database is a static JSON file because the app is designed for GitHub
Pages and has no application server. The file may be replaced by a larger,
versioned dataset later without changing the app entry point.
