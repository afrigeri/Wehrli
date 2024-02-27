
# Wehrli python module
1985 Wehrli Standard Extraterrestrial Solar Irradiance Spectrum, useful for processing Earth and Planetary mapping spectrometer data.

The 1985 Wehrli Standard Extraterrestrial Solar Irradiance Spectrum covers the solar spectrum from 199.5 nm to 10075.0 nm in increments increasing gradually from 1 nm in the shorter wavelengths to 2290 nm at the upper end of the spectrum.

```
import wehrli
import pandas as pd
import matplotlib.pyplot as plt

dataset = pd.DataFrame({'Wavelength': wehrli.wl_nm, 'W sm nm': wehrli.W_sm_nm, 'W sm': wehrli.W_sm })

dataset.plot.scatter(x="Wavelength",y="W sm")
plt.show()
```

### Reference

 * Wehrli, C. Extraterrestrial Solar Spectrum, Publication no. 615, Physikalisch-Meteorologisches Observatorium + World Radiation Center, Davos Dorf, Switzerland, July 1985.
