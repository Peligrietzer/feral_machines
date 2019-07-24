# Minimal Komologorov Complexity Music

## drone.c

I'm pretty happy with this one. There's an ominous cast to it, something that
makes me imagine a gathering army, in a Moebius-illustrated landscape. 

```c
#include <stdio.h>

void main(int t) {
  for (;;t++) {
    putchar(0xFA & (
          t 
          & t >> 6
          & ((t % (1 << 14)) < (1 << 13)? 
             t ^ (t >> 8)
             : t >> 8) 
          / (t <= 0? 1 : (1 + t % 32))
          ^ (t % 30)
          + ((t * (t>>18) * !(3 & t>>19)) & 0x0a)
          ^ ((t * (t>>19)) & 0xe1) 
          | ((t / 10) & (t >> 14) & (t>>15) & 0xaa)
        )
    );
  }
}
```

## Each bit, an instrument

## Compressibility

An interesting quirk about these tunes is that though they are of extremely
low _algorithmic_ complexity -- this is really the whole point of the genre
-- they often do _not_ compress elegantly into the standard audio container
formats. Their soundscape is irregular, jarringly textured, "noisy", in some
senseless way. 

[ mp3, etc. ]
