# Tissue_characterization
single_frequency and multi_frequency_data
Problem Statement: Joint learning of ultrasonic backscattering statistical physics and signal confidence
primal for tissue characterization with multi-frequency ultrasonic data.

Tasks done up till now:
* For single Frequency (5 MHz) US data.
- Single frequency ultrasound RF data acquisition from Verasonics machine.
- Data annotation (Total of three classes/labels: Hyperechoic, Hypoechoic, Background).
- Data-Frame creation with Scale and shape parameter estimation along with confidence map for
each data.
- Feeding the estimated data to random forest model to find semantic (pixel wise) segmentation.

For multi-frequency (5MHz to 10MHz in the interval of 0.5MHz) US data.
- Multi-frequency ultrasound RF data acquisition from Verasonics machine. Here each data has
higher variability than single frequency data. (each data contains data points from almost all
possible regions. (Total of three classes/labels/regions: Hyperechoic, Hypoechoic, Background).
- Data annotation (using Blender 3D software)
- As frequency increases the corresponding wavelength increases which eventually increases the
resolution of image that results in increase in data samples. Therefore size of image increases.
- Data-Frame creation with Scale and shape parameter estimation along with confidence map for
each data (by converging all frequency data to the dimensions of base frequency 5 MHz data).
- Feeding the estimated data to random forest model to find semantic (pixel wise) segmentation.
- Data-Frame creation (total of 11 Data-Frames each for different frequency) with Scale and shape
parameter estimation along with confidence map for each data.
- Feeding data to different random forest models (total of 11 each for different frequency) to find
semantic (pixel wise) segmentation.
