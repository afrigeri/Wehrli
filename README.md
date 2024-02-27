
# Wehrli python module
1985 Wehrli Standard Extraterrestrial Solar Irradiance Spectrum

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
