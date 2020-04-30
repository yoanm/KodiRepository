# KodiRepository
Kodi repository

Use https://github.com/Twilight0/Repository-Bootstrapper for generation

## How to add an addon
 - Link addon directory to root directory of this project (multiple addons allowed) :
   
   Example with `skin.unity.yo` addon : `ln -s ../skink.unity.yo .`

- Create a new version of YoanmRepo by following procedure below.
   
   TODO : Check if bumping repository version is mandatory ?!

## New repository version process
 - Replace current version on `YoanmRepo/addon.xml` by the new one. 
   
   Example with vi and version `1.1.0` to `1.2.0` : `:%s/1\.1\.0/1.2.0/`

- Replace current version on `_tools/config.ini` by the new one.
   
   Example with vi and version `1.1.0` to `1.2.0` : `:%s/1\.1\.0/1.2.0/`

- Run `./generate_repo.py`. 
  
  :warning: Command must be executed from `_tools` directory else it does not work ! :warning:
