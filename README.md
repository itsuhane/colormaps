# colormaps
Drop-in library for nice color-maps in C++
Currently, color-maps are from [CET Perceptually Uniform Colour Maps](http://peterkovesi.com/projects/colourmaps/).

## Usage
Simply include `colormaps.h` and use desired color-maps.

Example:
```cpp
#include <colormaps.h>
using colormaps::rgb_color;                      // just std::array<double, 3>
auto colormap = colormap::linear::kryw_0_97_c73; // pick color-map

double x = 0.7;                                  // value in [0,1]
rgb_color color = colormap(x);                   // (r,g,b) values in [0,1]^3
```
