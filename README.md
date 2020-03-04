# Hairy-Slices-II-Data
The dataset, results, and statistical analyses from the paper "Hairy Slices II: Depth Cues for Visualizing 3D Streamlines Through Cutting Planes" by Stevens et al., 2020


## Format for hairy_slices_ii_data.bov

```c
FILE *inputFile = fopen("hairy_slices_ii_data.bov", "rb");

int nXPoints, nYPoints, nZPoints;

nXPoints = nYPoints = nZPoints = 400;

for (int x = 0; x < nXPoints; x++) {
    for (int y = 0; y < nYPoints; y++) {
        for (int z = 0; z < nZPoints; z++) {
            float u, v, w;
            fread(&u, sizeof(float), 1, inputFile);
            fread(&v, sizeof(float), 1, inputFile);
            fread(&w, sizeof(float), 1, inputFile);
            // now store uvw vector in preferred data structure
        }
    }
}
```
