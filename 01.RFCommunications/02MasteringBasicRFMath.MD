# Mastering Basic RF Math

### Watts, Milliwatts, dBi (Decible Scale), dBm (Decible Milliwatts)

**Watts:** Watts is a measure of electical energy. How much electrical energy consume, how much electrical energy sent or how much electrical energy receive.

**Milliwatts:** A thousandth watt is a milliwatt.

*A radio station can be broadcast 50,000 watts.*
*Microwave oevn: 1000 watts.*
*Wi-Fi AP: 1 to 100mW.*

**The Decible Scale:** Initially designed to compare sounds values, but can compare any powers as long as we add the unit to "db", to show that the reference is.


### Comparing Antenna Power in Terms of dBi and dBd

Antenna's range is calculating mW. There no electricity comming out the Antenna. There is electromagnetic field but it is just an potential.

**Isotropic Antennae**
	- 1 dot large.
	- Sends exactly the same energy in all directions.
	- dBi scale
	- It's does not exists in real workd.

**Dipolse Antienna**
	- Referse to dipole (AKA "rubber duck")
	- Simplest real word antenna.
	- 0 dBd = 2.14 dBi
	- Logarithm scale same as the orther dB scales


### Calculations with Laws of 3s and 10s

**Convert mW (Milliwatts) to dBm  (Decible Milliwatts)**

```
1 mW	= 0 dBm
10 mW	= 10 dBm
100 mW	= 20 dBm
200 mW	= 23 dBm
300 mW	= 17 dBm
```

*Everytime We multiple by 10 that's means we add 10 dBm.*

*Everytime we multiple by 2 that's means we add 3 dBm*

*Everytime we devide by 2 that's means we remove 3 dBm*

**Convert dBm  (Decible Milliwatts) to mW (Milliwatts)**

```
30 dBm	= ? mW

1	x 10	= 10 dBm
10	x 10	= 10 dBm
-------------------------
			= 20 dBm
10 x 10 mW	= + 10 dBm
-------------------------
			= 30 dBm
100	x 10	= 1000 mW

36 dBm = ? mW
```

*As we know the rule that, when we add double dBm then we multiple by 2 mW*

```
30 dBm	= 3000 mW
33 dBm	=> 1000 mW	x 2 = 2000 mW
36 dBm	=> 2000 mW	x 2	= 400 mW
```

Now what abotu -50 dBm = ? mW

```
0 dBm	= 1 mW
10 dBm	= (1/10) 0.1 mW
10 dBm	= 0.01 mW
10 dBm	= 0.001 mW
10 dBm	= 0.0001 mW
10 dBm	= 0.00001 mW
```

### Effective Isotropic Radiated Power (EIRP)

![EIRP](https://raw.githubusercontent.com/jakiiii/WirelessNetworking/master/Images/eirp.jpg)

**EIRP (dBm) = Tx Power (dBm) - cable loss (dB) + Antenna Gain (dBi)**

Example:
```
Tx Power = 20 dBm, loss 3dB, anteena gain = 6 dBi
EIRP = 20 - 3 + 6 = 23 dBm
```

### Mastering Basic RF Math

