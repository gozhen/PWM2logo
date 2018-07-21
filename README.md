PWM2logo is a simple tool to draw DNA sequence logo from Position weight matrix (PWM). PWM2logo is written in Python. 


## Tutorial

./demo_files/demo_pwm.csv
```
	0.304348,	0.068966,	0.950000,	0.990000,	0.156250,	0.690000,	0.285714,	0.480000,	0.100000,	0.066538,	0.033333,	0.053261,	0.010000,	0.065000,
	0.600000,	0.000517,	0.016667,	0.003333,	0.710000,	0.042097,	0.152143,	0.169091,	0.160000,	0.066538,	0.013333,	0.053261,	0.860000,	0.065000,
	0.047826,	0.930000,	0.016667,	0.003333,	0.066875,	0.225806,	0.152143,	0.169091,	0.100000,	0.790000,	0.013333,	0.043478,	0.010000,	0.630000,
	0.047826,	0.000517,	0.016667,	0.003333,	0.066875,	0.042097,	0.410000,	0.181818,	0.640000,	0.076923,	0.940000,	0.850000,	0.120000,	0.240000,
```
demo_pwm.csv is a file storing the PWM, where four rows represent the probabilities for 'A', 'C', 'G' and 'T' respectively, multiple columns, each representing a nucleotide position. 

Run code below:
```
import pwm2logo
fn_csv = './demo_pwm.csv'
pwm2logo.f_draw_logo_from_pwm(fn_csv)
```
The sequence logo image file is genereted under the same folder:
![demo_logo](https://github.com/gozhen/PWM2logo/blob/master/demo_files/demo_logo.png)



## Acknowledgements  

Thanks for ImportanceOfBeingErnes and rightskewed from this thread:
  https://stackoverflow.com/questions/42615527/sequence-logos-in-matplotlib-aligning-xticks



