# 26.1.2-farlands-fabric
1.18+ world generation was completely reworked, so in newer versions farlands look different, though the noise overflow is still possible for fun shapes. 1.18 uses 3d noise generation that is not affected by the same bug from beta 1.7.3

also coordinates are no longer used as pure int values, rather they're passed through a single long value with only 26 bits for x/z (x/z - 26 bits each, y - 12) for the sake of optimisation, so the limit is way lower than pre-1.18 2+ billions (2^31). This version crashed when trying to generate chunks past 2^25 (around 33mil) so no fartherlands

ofc written by ai, looks like it was harder to make out new mojang code, but its clear that the world gen changed a ton, so even though the terrain changes, it stays relatively sane. 
