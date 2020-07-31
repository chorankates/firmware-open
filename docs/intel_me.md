# Intel Management Engine

The IME is present, but disabled. This is accomplished by [sending a HECI
command on boot][heci_disable], before RAM is initalized. This puts the IME in
a state similar to setting the HAP bit on earlier platforms. [me_cleaner] is
not used as it does not support IME version 14.0.

[heci_disable]: https://github.com/system76/coreboot/blob/f3ba5937e778105cb7e75de9a1d4adf54ea825e5/src/soc/intel/cannonlake/me.c#L186
[me_cleaner]:https://github.com/corna/me_cleaner
