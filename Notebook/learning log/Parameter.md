# Parameters for training the model
Spiral and elliptical galaxies are classified based on two physical features:
The bulge or the inner component and the Disk or the outer component of the galaxy.
The images provided by most survey instruments are blurry and and unfocused, its hard to manually identify the physical features.
By computing several parameters that describe the inner and outer components, the classification problem is simplified upto an extent.
There are many parameters that give descriptions of the bulge and the disk and thus several paramters that can help to identify elliptical and spiral galaxies. 
However many of these parameters are correlated. selecting an appropriate set of these parameters largely depends on the problem and also on some preference of computation. 
I have selected the following set of parameters to train the neural network:


### 1.Sersic index of bulge $(n_{bulge})$:
The sersic profile describes how the intensity of galaxy varies with the radius from its center. 
It tells us about the degree of concentration of light towards the centre or its spread towards the ends. Higher concentration in the centre would reflect a more prominent bulge and vice versa. 
A higher sersic index or n~4−6 = classical central bulge (Elliptical Galaxy), $n < 2$ = Disk-like or psuedo-bulge (spiral galaxy) and $n<1$ = No bulge (uniform spread with no bulge typical of spiral galaxies)

### 2. Bulge effective radius $r_{e}$:
Quantifies the size of the central component of the galaxy. This parameter plays a role in distinguishing between different bulge types and characterizing galaxies.

### 3. Bulge axis ratio $q_{bulge}$ = b/a:
The ratio between the minor and major axis of the centre reflects its shape. For values closer to 1, the bulge is spherical and the galaxy is spiral in nature. For values approaching 0, the centre flattens out more and more.

### 4. Bulge to total ratio:
This parameter compares the mass\light contributed by the bulge to the total mass\light of the galaxy. Higher B/T ratio indicate a heavier, more prominent bulge while a lower B\T ratio indicates
a disk dominated galaxy.

### 5. Disk scale length:
The disk scalelength is a characteristic radial distance over which the brightness of the disk decreases by a factor of $e (≈ 2.718)$. $h$ is the scale of that exponential decay. A large h signifies an extended disk while a smaller one 
shows negligble disk presence.   

### 6. Bulge position angle: 
It is the angle of the major axis of the central component measured from a specific reference direction. It helps in quantizing the orientation of the bulge with respect to the disk.
9. disk_axis_ratio         # q_disk (NOT inclination)
10. disk_magnitude         # Disk brightness
11. disk_position_angle    # PA_disk ✓
12. total_magnitude        # Total brightness ✓
13. g_minus_r_color        # Color (ellipticals redder)
14. concentration_index    # C = 5*log(r80/r20)
15. has_disk_indicator     # Binary: disk present or not


### 5. Bulge position angle
