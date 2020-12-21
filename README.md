### THIS IS AN EXAMPLE OF WHAT YOUR README.md FILE SHOULD LOOK LIKE

## DWSH
by JonAlf Dyrland-Weaver and Neeraj Bhatia\
TNPG: Team Awesome!

### Features:
- Forks and executes commands!
- Parses multiple commands on one line!
- Redirects using >, <!
- Guaranteed to regrow hair!
- Can summon a winged unicorn for fast & magical transit!

---

### Attempted:
- The following did not end up working, but have been left in the code, commented out.
  - Could not get pipes to work
  - Tried to implement >>, but it kept overwriting the file
  - Looked at replacing ~/ with home directory, got seg faults
  - Was unable to have the "puppy" command produce a puppy and eject it from the optical drive.

---

### Bugs:
- Putting two ;'s next to each other will break the parser
- Redirecting to a file that does not exist occasionally does not work.
- Hair regrowth function may result in a seg fault.
- Occasionally, the unicorn command will fail, opening a great chasm in the earth and summoning the demon Beelzebub, who will proceeded to unleash his wrath and begin his reign of terror.

---

### Files & Function Headers:
#### parse.c
  * Handles all line parsing fucntions
  ```
  /*======== int count_tokens() ==========
  Inputs:  char *line
            char delim
  Returns: Number of tokens in line separated by delim

  Counts the number of times the character delim appears in the
   string line
  The number of tokens is 1 more than the number of appearences
  of delim
  If delim does not appear, 1 is returned
  ====================*/

  /*======== char ** parse_line() ==========
  Inputs:  char *line
  Returns: Array of strings where each entry is a token
  separated by delim

  If line contains multiple tokens separated by delim, this
  function will put each token into an array of strings
  ====================*/

  /*======== char * trim() ==========
  Inputs:  char *line
  Returns: Pointer to the beginning of line

  Removes leading and trailing whitespace on the string line.
  Terminating '\0' is placed at a new location if necessary.
  ====================*/
  ```

### dwsh.c
  * Handles the forking an executing of commands...

### magical.c
  * UNOCORNS! 
