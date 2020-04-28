# rpg_in_lisp
that's my game's learning, it was made when I was in chapter 6 of land of Lisp, soon I'll add a CLI, and won't continue to use CLISP either :P

# How to use
To use that script, on the same directory that you've downloaded the script, run either sbcl or clisp, and then:

`(load "game.lisp")`

For now on, you can test the functions and the beta version of the game :), see an example:

```
$ sbcl
* (load "game.lisp")
T
* (look)
(YOU ARE IN THE LIVING-ROOM. A WIZARD IS SNORING LOUDLY ON THE COUCH. THERE IS
 A DOOR GOING WEST FROM HERE. THERE IS A LADDER GOING UPSTAIRS FROM HERE. YOU
 SEE A WHISKEY ON THE FLOOR. YOU SEE A BUCKET ON THE FLOOR.)
* (pickup 'bucket)
(YOU ARE CARRYING THE BUCKET)
* (inventory)
(ITEMS- BUCKET)
* (look)
(YOU ARE IN THE LIVING-ROOM. A WIZARD IS SNORING LOUDLY ON THE COUCH. THERE IS
 A DOOR GOING WEST FROM HERE. THERE IS A LADDER GOING UPSTAIRS FROM HERE. YOU
 SEE A WHISKEY ON THE FLOOR.)
* (walk 'ladder)
(YOU CANNOT GO THAT WAY.)
* (walk 'west)
(YOU ARE IN A BEAUTIFUL GARDEN. THERE IS A WELL IN FRONT OF YOU. THERE IS A
 DOOR GOING EAST FROM HERE. YOU SEE A FROG ON THE FLOOR. YOU SEE A CHAIN ON THE
 FLOOR.)
* (pickup 'frog)
(YOU ARE CARRYING THE FROG)
* (inventory)
(ITEMS- BUCKET FROG)
* (walk 'door)
(YOU CANNOT GO THAT WAY.)
* (walk 'east)
(YOU ARE IN THE LIVING-ROOM. A WIZARD IS SNORING LOUDLY ON THE COUCH. THERE IS
 A DOOR GOING WEST FROM HERE. THERE IS A LADDER GOING UPSTAIRS FROM HERE. YOU
 SEE A WHISKEY ON THE FLOOR.)
 ```

 Or simply... You can do:

 `$ clisp cli.lisp`

 I've seen errors on sbcl's flush.

**For now on, I'll back down my decision to use CLISP, and I can't ensure that it'll work perfectly, don't beat up me hahaha :)**
