# WhatsMyName
This repository has the unified data required to perform user and username enumeration on various websites. Content is in a JSON file and can easily be used in other projects such as the ones below:

![whatsmyname](whatsmyname.png)

[![Open Source](https://img.shields.io/badge/Open%20Source-100%25-green.svg)](https://shields.io/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-Yes-green.svg)](https://github.com/GetStream/winds/graphs/commit-activity)
[![Version](https://img.shields.io/badge/Version-1.6-orange)](https://github.com/GetStream/winds/graphs/commit-activity)

* https://whatsmyname.app/ - [Chris Poulter](https://twitter.com/osintcombine) created this site which draws the project's JSON file into a gorgeous and easy to use web interface.
  * There are no ads.
  * He does not collect what you search for
  * Filters for category and in search results
  * FAST!
  * Pulls the lastest version of the project's JSON file when run.
* [Recon-ng](https://bitbucket.org/LaNMaSteR53/recon-ng) - The [Profiler Module](https://bitbucket.org/LaNMaSteR53/recon-ng/src/7723096ce2301092906838ef73564e7907886748/modules/recon/profiles-profiles/profiler.py?at=master&fileviewer=file-view-default) grabs this JSON file and uses it. See https://webbreacher.com/2014/12/11/recon-ng-profiler-module/ for details.
* [Spiderfoot](https://github.com/smicallef/spiderfoot) uses this in the [sfp_account](https://github.com/smicallef/spiderfoot/blob/master/modules/sfp_accounts.py) module. There is also [this video](https://asciinema.org/a/295923) showing how to use this project using the Spiderfoot Command Line Interface (CLI).
* [sn0int](https://github.com/kpcyrd/sn0int) downloads and uses the JSON file in the [kpcyrd/whatsmyname](https://sn0int.com/r/kpcyrd/whatsmyname) module, see https://twitter.com/sn0int/status/1228046880459907073 for details and instructions.


# Format

See [CONTRIBUTING](CONTRIBUTING.md)

# Standalone Checker
If you just want to run this script to check user names on sites and don't wish to use it in combination with another tool (like Recon-NG and/or Spiderfoot), then you can use the included Python 3 script as shown below:

```
 $  python3 ./web_accounts_list_checker.py -u sdfsfsdfsdfs
 -  161 sites found in file.
 -  Found user at http://www.break.com/user/sdfsfsdfsdfs
      ! ERROR: CONNECTION TIME OUT. Try increasing the timeout delay.
 -  Found user at https://klout.com/sdfsfsdfsdfs
 -  Found user at https://social.technet.microsoft.com/profile/sdfsfsdfsdfs/
 -  Found user at https://www.pinterest.com/sdfsfsdfsdfs/
 -  Found user at https://www.reddit.com/user/sdfsfsdfsdfs
 -  Found user at http://scratch.mit.edu/users/sdfsfsdfsdfs/
 *  Skipping Slashdot - Marked as not valid.
 *  Skipping SmiteGuru - Marked as not valid.
 *  Skipping SoundCloud - Marked as not valid.
 -  Found user at http://steamcommunity.com/id/sdfsfsdfsdfs
 -  Found user at http://www.tf2items.com/id/sdfsfsdfsdfs/
 -  Found user at https://twitter.com/sdfsfsdfsdfs
 -  Found user at http://videolike.org/video/sdfsfsdfsdfs
      ! ERROR: CONNECTION TIME OUT. Try increasing the timeout delay.
 -  Found user at http://www.xvideos.com/profiles/sdfsfsdfsdfs
```

There is a bash script `whatsmyname.sh` in the repository that uses Zenity to run the Python standalone checker.

# Updates
I update this project as I have time and would *LOVE* to have interested people help maintain and grow it. Please reach to me webbreacher {at} protonmail {dot} com if you are interested.

# Contributors
[@WebBreacher](https://github.com/WebBreacher/)<br>
[@Munchko](https://github.com/Munchko/)<br>
[@L0r3m1p5um](https://github.com/L0r3m1p5um/)<br>
[@lehuff](https://github.com/lehuff/)<br>
[@arnydo](https://github.com/arnydo)<br>
[@janbinx](https://github.com/janbinx/)<br>
[@bcoles](https://github.com/bcoles)<br>
[@Sector035](https://github.com/sector035/)<br>
[@mccartney](https://github.com/mccartney)<br>
[@salaheldin](https://github.com/salaheldinaz)<br>

# License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
