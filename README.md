# covid_dk_plot
Timeseries plot of Covid-19 cases in Denmark. Built in Python, and produces [this output video](https://github.com/mrath/covid_dk_plot/raw/master/covid_dk.mp4).

Data is avilable near the bottom of [this web page](https://www.ssi.dk/sygdomme-beredskab-og-forskning/sygdomsovervaagning/c/covid19-overvaagning), updated daily (14.00 CET). Just download and unzip to the `data` directory. 

The code is available in a [Jupyter Notebook](covid_dk_plot.ipynb). The [Python script](covid_dk_plot.py) extracted from the notebook should also be up to date with the content of the notebook. 

When running the code, a plot will be made for each day in the dataset as a PNG file in the `out` directory. These plots can be combined in a video using the `make_video.sh` script.

**NOTE:** The plotting routine (generating the PNGs) takes a long time currently (1hr+ for 200 plots). Haven't really bothered figuring out why, since I didn't spend a lot of time on this. But now you know. 


## Dependencies
- Jupyter notebook
- `ffmpeg` to create the video
- Python modules:
  - `pandas`
  - `matplotlib`
  - `geopandas`
  - `numpy`
  - `contextily` (optional)

