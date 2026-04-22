# AS-umbra-flood
Scripts used in flood/coastline detection for American Samoa using imagery from Umbra space.

Jupyter notebooks:
- "cluster_geotiff_auto_FINAL.ipynb": Main utility for extracting coastlines from GAMMA-generated RTC geotiff imagery. Any geotiff file can be used - does not have to be GAMMA RTC. GEC can also be used, but performance is significantly worse than using GAMMA-generated RTC imagery.

- "plot_umbra_conf_matrix.ipynb": Plots Umbra confusion matrix for flood detection.

- "get_umbra_flood.ipynb": Generate Umbra flood maps from land/water binary mask.

- "plot_umbra_mask_comp.ipynb": Plots quality statistics related to Umbra land/water masking.

- "run_length_buffer_cmp_umbra.ipynb": Run buffer analysis on Umbra imagery coastline detection compared with a reference landcover file.

- "get_rainfall.ipynb": Get rainfall data from Vaitipo Station (UH Mesonet Live Data) at dates from a *csv file of Umbra acquisition capture times "Capture_Times.csv".

- "get_tg_height.ipynb": Extracts Pago Pago tide gauge height (default in ft) from a *csv file of Umbra acquisition capture times "Capture_Times.csv".

- "get_tg_height_uh.ipynb": Same as previous but with tide gauge data from UH.
  
- "reproject_umbra_GEC.ipynb": Utility for generating RPC-corrected GEC imagery. A DEM covering the AOI is needed.

CSV files:
- "CO-OPS_1770000_wl.csv": Tide gauge levels at Pago Pago downloaded from the NOAA Inundation History website at https://tidesandcurrents.noaa.gov/inundationdb/inundation.html?id=1770000.
- "Capture_Times.csv": Capture times of Umbra acquisitions.
- "Capture_Times_LocalTime.csv": Capture times of Umbra acquisitions in local time (SST).

XLSX files:
- "Umbra Data Inventory FINAL - AS.xlsx": Inventory of all Umbra data acquired for each area of interest as part of the CSDA study, including unused imagery. Details of satellite parameters and events of interest are included.

Misc files: 
- "ChatGSFC_GeoTIFF_K-Means Clustering Code.txt" and "Filtering_Water Mask Coastline Contours.txt": Export of ChatGSFC prompts and responses used as part of creating "cluster_geotiff_auto_FINAL.ipynb".
- "Confusion_Matrix Plot Template.txt" Export of ChatGSFC prompts and responses used as part of creating "plot_umbra_conf_matrix.ipynb"
- "Flood_Map Generation From Water Masks.txt" Export of ChatGSFC prompts and responses used as part of creating "get_umbra_flood.ipynb"
- "Land-Water_Mask Accuracy Evaluation.txt" Export of ChatGSFC prompts and responses used as part of creating "plot_umbra_mask_comp.ipynb"
- "SAR_Coastline Length And Buffer Analysis.txt" Export of ChatGSFC prompts and responses used as part of creating "run_length_buffer_cmp_umbra.ipynb"

THIS IS RESEARCH CODE PROVIDED TO YOU "AS IS" WITH NO WARRANTIES OF CORRECTNESS. USE AT YOUR OWN RISK.
