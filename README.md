Natural Tree Expansion -- A Mod for Factorio v0.14
========================================

Update 3.2 - Multiplayer desync fixed

* Instigated by CobaltEcho with Daniel34 doing most of the work!

* Multiplayer desync issue should be corrected.  I have tested on multiplayer and seems to be working.  Also upped the spawn rate of the trees.

* Forum notes at: https://forums.factorio.com/viewtopic.php?f=25&t=42313

========================================

Update 3.0 and 3.1

* Failed attempts at fixing multiplayer desync.

========================================

Orignal post by msakuta:

This mod will make trees automatically reproduce and expand over time.
The growth rate is very low (otherwise you'd drown in forest in long game),
but you can configure it in config.lua if you want.

Other things being worth noting are:

* There's a hard limit on tree count, whose default value is 800000, so
your save file won't get super-heavy.

* Trees won't grow on sand, stone path or concrete, so pave your base to prevent
them from entering.

* Trees too far from any of player's entities (about 192 tiles) won't grow,
because it would make the game and save file unnecessarily heavy.

* Debug mode shows count of existing trees and trees which have been added.

* Multiplayer is not tested. This mod uses Lua's math.random(), which could
cause problems on multiplayer game and replays.

* Although this mod gradually processes all trees in the game, the algorithm is
highly optimized so that execution time per tick is very low.
You won't feel a 'micro freeze' unless the game is very big.

Now get your flamethrower ready!
