
# Spatio-Temporal Atlas of Fetal Brain White Matter Tracts

This repository contains a spatio-temporal atlas of white matter tracts in the fetal brain, covering gestational ages from 23 to 36 weeks. This atlas maps the development of white matter tracts and provides insights into the dynamic changes in the fetal brain's architecture. This atlas can be a valuable resource for neuroscience research and clinical applications.

## Project Structure

The repository is organized into directories by gestational age (GA) and contains several types of files, as outlined below:

```
Fetal_tract_atlas/
├── GA{gestational_age}/
│   ├── diffusion/
│   │   ├── GA{gestational_age}_cfa.nii.gz
│   │   ├── GA{gestational_age}_fa.nii.gz
│   │   ├── GA{gestational_age}_md.nii.gz
│   │   └── GA{gestational_age}_tensor.nii.gz
│   ├── masks/
│   │   ├── GA{gestational_age}_{tract}_mask.nii.gz
│   │   └── ... (other masks for specific tracts)
│   ├── segmentation/
│   │   ├── GA{gestational_age}_5tt.nii.gz
│   │   └── GA{gestational_age}_seg.nii.gz
│   └── tracts/
│       ├── GA{gestational_age}_{tract}.trk
│       └── ... (other tract files for specific tracts)
├── metadata/
│   ├── Tracts_orientation.csv
│   └── Tracts_color_map.csv
```

## Directory and File Description

- **GA{gestational_age}/**: Contains subfolders for each gestational age with relevant data files:
  - **diffusion/**: Diffusion images, including color-code fractional fnisotropy (cfa), Fractional Anisotropy (fa), mean diffusivity (md), and tensor map files.
  - **masks/**: Binary masks for specific white matter tracts.
  - **segmentation/**: Five-tissue type maps (5tt) and segmentation (seg) files.
  - **tracts/**: Tractography files in `.trk` format representing white matter tracts.
  
- **metadata/**: Additional data files used in visualizing and analyzing the atlas:
  - **Tracts_orientation.csv**: Specifies the direction of streamlines for each tract.
  - **Tracts_color_map.csv**: Details the color map used for atlas visualization.

## Data Overview

The atlas includes data on 60 distinct white matter tracts.

## Installation and Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/Fetal_tract_atlas.git
   ```
2. **Data Visualization**:
   - Use software such as FSLeyes or ITK-SNAP for viewing `.nii.gz` files.
   - TrackVis can be used for visualizing `.trk` files.
3. **Referencing the Atlas**:
   - For more details on how the atlas was created, please refer to [Calixto et al. (2024)](https://doi.org/10.1073/pnas.XXXXXXXXXX).

## References

If you use this atlas, please cite the original publication:
> Calixto, C., et al. (2024). A detailed spatio-temporal atlas of the white matter tracts for the fetal brain. *Proceedings of the National Academy of Sciences*. DOI: XXXXXXXXXX.
