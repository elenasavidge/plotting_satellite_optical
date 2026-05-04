# plotting_satellite_optical

Notebook for plotting and comparing optical satellite scenes (Sentinel-2, Landsat 8, MODIS) over a polar AOI.

- `compare_satellite_scenes.ipynb` — side-by-side scene comparison with RGB composites from raw bands.

See `environment.yml` for dependencies.

## Data

Drop files into the layout below. Exact files used in the notebook:

```
data/
├── Landsat8/
│   ├── LC08_L2SR_061113_20181014_20201016_02_T2_SR_B2.TIF
│   ├── LC08_L2SR_061113_20181014_20201016_02_T2_SR_B3.TIF
│   └── LC08_L2SR_061113_20181014_20201016_02_T2_SR_B4.TIF
├── sentinel2/
│   └── 20181017/
│       ├── T58CDB_20181017T211529_B02.jp2
│       ├── T58CDB_20181017T211529_B03.jp2
│       └── T58CDB_20181017T211529_B04.jp2
└── MODIS/
    ├── A2018288/MYD09.A2018288.1325.061.2021343103158.hdf
    └── A2018290/
        ├── MYD09.A2018290.0820.061.2021343114527.hdf
        └── MYD09.A2018290.1135.061.2021343113632.hdf
```

### Where to download

- **Landsat 8 Collection 2 L2 SR** — USGS EarthExplorer (`earthexplorer.usgs.gov`). Search path/row 061/113, 2018-10-14.
- **Sentinel-2 L1C** — Copernicus Browser (`browser.dataspace.copernicus.eu`). Tile T58CDB, 2018-10-17.
- **MODIS Aqua MYD09GA** — NASA LAADS DAAC (`ladsweb.modaps.eosdis.nasa.gov`). Granules A2018288 and A2018290.
