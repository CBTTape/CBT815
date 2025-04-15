# CBT815
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 815 is from Bob Glover and contains an extended string    *   FILE 815
//*           search facility that runs under ISPF.  We trust that  *   FILE 815
//*           it will be useful to you.                             *   FILE 815
//*                                                                 *   FILE 815
//*           email:  "Glover, Bob" <im4fsu@comcast.net>            *   FILE 815
//*                                                                 *   FILE 815
//*     The following is a description of this facility in          *   FILE 815
//*     more detail.                                                *   FILE 815
//*                                                                 *   FILE 815
//*     SRCHE                                                       *   FILE 815
//*                                                                 *   FILE 815
//*     This is a search facility that supports the searching of    *   FILE 815
//*     a user entered variable across multiple datasets.  It       *   FILE 815
//*     consists of (1) REXX and (3) ISPF panels.  It is an         *   FILE 815
//*     enhancement to the already CBT present SRCH facility        *   FILE 815
//*     which I introduced many years ago.  The core code was       *   FILE 815
//*     created by Lee Hayden. I created the logic that wraps       *   FILE 815
//*     around it.                                                  *   FILE 815
//*                                                                 *   FILE 815
//*     Users interface with SRCHE (SRCH EXTENDED) in two ways,     *   FILE 815
//*     both in TSO/E. ONE: simply issue  TSO SRCHE  and a panel    *   FILE 815
//*     pops up to allow one to enter any dataset name search       *   FILE 815
//*     mask. TWO: on a  3.4  screen showing one or more dataset    *   FILE 815
//*     names, enter  SRCHE  on a dsname line and the same panel    *   FILE 815
//*     pops up with that name in its dsname mask. At this point    *   FILE 815
//*     users can modify the panel dsname to whatever they want.    *   FILE 815
//*                                                                 *   FILE 815
//*     A main issue with doing all this is that one may            *   FILE 815
//*     inadvertently request one (or many) DFHSM MIGRATED          *   FILE 815
//*     datasets to appear as potential search targets. SRCHE       *   FILE 815
//*     presents a list of all MIGRATED datasets so the user can    *   FILE 815
//*     rethink his/her search mask. SRCHE will NOT issue any       *   FILE 815
//*     RECALLS. This must be done by the user. Once a valid        *   FILE 815
//*     list of target datasets has been created, SRCHE will        *   FILE 815
//*     then act like SRCH and ask the user for a valid search      *   FILE 815
//*     argument to go against the list of datasets previously      *   FILE 815
//*     created. A maximum of 5,000 hits is supported but that      *   FILE 815
//*     can easily be changed in the REXX.  The only limitation     *   FILE 815
//*     is the size of a TSO user's region.                         *   FILE 815
//*                                                                 *   FILE 815
```
