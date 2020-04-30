# KodiRepository
Kodi repository

Use https://github.com/Twilight0/Repository-Bootstrapper for generation

## How to add an addon
 - Link addon directory to root directory of this project (multiple addons allowed) :
   
   Example with `skin.unity.yo` addon : `ln -s ../skink.unity.yo .`

- Create a new version of YoanmRepo using process described below.
   
   TODO : Check if bumping repository version is mandatory ?!

N.B.: Same procedure works for addons updates

## New repository version process
 - Replace current version on `YoanmRepo/addon.xml` by the new one. 
 - Replace current version on `_tools/config.ini` by the new one.
 - Run `./generate_repo.py`. 
  
  :warning: Command must be executed from `_tools` directory else it does not work ! :warning:
