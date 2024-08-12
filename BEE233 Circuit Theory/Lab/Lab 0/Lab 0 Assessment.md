# Lab 0-1
$f = 1kHz$
$V_p = 1V$
$V_{pp} = 2V$
$T = 1_{ms}$
$V_{dc} = 1V$
$Div = 500mV ea.$
$\phi = 0$

$V_p = \frac{Volts}{Div} = \frac{1V}{500mV * 2} = 1V$
$V_p = 1V$
$V_{pp} = Amplitude = 2*mag = \frac{Volts}{Div}*2 = 1V*2 = 2V$
$V_{dc} = V_{pp} - V_p = 2V - 1V = 1V$
$T=\frac{Sec}{Div} = 2.5*400=1ms$
$\frac{1}{T} = \frac{1}{1_{ms}} = 1kHz$
$w=2\pi f = 2\pi * 1000Hz = 2000\pi \frac{rads}{s}$
$v(t) = V_p + cos(\omega*t - \phi)= 1V + cos(2k\pi*t)$
![[tek00001.png]]
# Lab 0-2
$f = 1kHz$
$\phi + 45\degree$
$V_{pp} = 2V$
$Offset = 0$
$T = 1ms$
$\Delta t = \frac{3}{5}*\approx tick*Div(200\mu s) = 120\mu s$
$\Delta \phi = \frac{\Delta t}{T} * 360\degree = \frac{120\mu s}{1ms}*360\degree = 43.2\degree$
$V_1 = A*cos(\omega*t - \phi) = 500mv*cos(2000\pi*t)$
$V_2 = 250mV*cos(200\pi*t + 45\degree)-250*45\degree mV$
$\Delta t = \frac{45\degree}{1300\degree*1kHz} = 0.125ms$![[tek00004.png]]