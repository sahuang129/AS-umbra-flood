# AS-umbra-flood
Scripts used in flood/coastline detection for American Samoa using imagery from Umbra space.

Jupyter notebooks:
- "cluster_geotiff.ipynb": Main utility for extracting coastlines from GAMMA-generated RTC geotiff imagery. Any geotiff file can be used - does not have to be GAMMA RTC. GEC can also be used, but performance is significantly worse than using GAMMA-generated RTC imagery.

- "get_rainfall.ipynb": Get rainfall data from Vaitipo Station at dates from "Capture_Times.csv".

- "get_tg_height.ipynb": Extracts Pago Pago tide gauge height (default in ft) for a *csv file of Umbra acquisition capture times. "Capture_Times.csv" included. 

- "get_tg_height_uh.ipynb": Same as 1) but with tide gauge data from UH
  
- "reproject_umbra_GEC.ipynb": Utility for generating RPC-corrected GEC imagery. A DEM covering the AOI is needed.
