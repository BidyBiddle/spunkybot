This README is just a quick start document. You can find more detailed documentation at [https://spunkybot.de](https://spunkybot.de).

# What is Spunky Bot?

**Spunky Bot** is a lightweight game server administration bot and RCON tool.
Its purpose is to administrate an [Urban Terror](http://www.urbanterror.info) 4.1 / 4.2 server and to provide real time statistical data for players.
Spunky Bot offers in-game commands without authentication and automated administration even when no admin is online.
The code of Spunky Bot is inspired by the eb2k9 bot by Shawn Haggard, which was released under the Beerware License.

[![Build Status](https://travis-ci.org/SpunkyBot/spunkybot.png?branch=master)](https://travis-ci.org/SpunkyBot/spunkybot)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.5.0-orange.svg)

If you want to know more, this is a list of selected starting points:

* Introduction to [Spunky Bot](https://spunkybot.de)
* The full list of [commands](https://github.com/SpunkyBot/spunkybot/blob/master/doc/Commands.md)
* There is much more inside the [official documentation](https://github.com/SpunkyBot/spunkybot/wiki)


## Features
- Lightweight and fast
- Real time game statistics
- Different user groups and levels
- Supports all RCON commands
- Supports temporary and permanent bans of players
- Supports rotation messages
- Stores all player related information in a SQLite database
- Runs 'out of the box', no other software requirements


## Environment
- Urban Terror 4.1.1 and 4.2.023
- Python 2.6.x / 2.7.x
- SQLite 3 database
- Linux platform (tested on Debian 6 & 7, Ubuntu 12 & 14, CentOS 6.5 and Mac OS X 10.10)
- Supporting Linux 32-bit and 64-bit operating system


## Quickstart
It's easy to get started with Spunky Bot:

- Download the [latest release](https://spunkybot.de/#download)
- Read our [quickstart guide](https://spunkybot.de/#get-started) to get up and running

### Configuration
- Modify the Urban Terror server config file as follows:
	- `seta g_logsync "1"`
	- `seta g_loghits "1"`
- Restart your Urban Terror server
- Modify the Spunky Bot configuration file `/conf/settings.conf` and set game server port and RCON password
- In-game displayed rules/advertisements are contained in the file `/conf/rules.conf`
	- If you do not want to display the rotation messages, set the value `show_rules=0` in the config file `/conf/settings.conf`
- Run the application manually: `python spunky.py`
- Or use the provided initscript to run Spunky Bot as daemon

**_First start instruction:_**

- Connect to your game server and type `!iamgod` in the global chat to get the admin level "Head Admin". This command is only once available.


## Documentation
You can find all the documentation in the [Wiki](https://github.com/SpunkyBot/spunkybot/wiki).

### Bot Commands
The description of all available [commands](https://github.com/SpunkyBot/spunkybot/blob/master/doc/Commands.md) as well as the admin levels and rights is located under the subfolder `/doc`.


## Resources
* [Documentation](https://github.com/SpunkyBot/spunkybot/wiki)
* [Troubleshooting](https://github.com/SpunkyBot/spunkybot/wiki/Troubleshooting)
* [Bug Tracker](https://github.com/SpunkyBot/spunkybot/issues)
* [Mailing List](https://groups.google.com/group/spunkybot)
* [Code](https://github.com/SpunkyBot/spunkybot)
* [Homepage](https://spunkybot.de)


## Changelog
You can keep up-to-date with the changes that we have made via our [releases page](https://github.com/Spunkybot/spunkybot/releases).


## Versioning
Spunky Bot is currently maintained under the [Semantic Versioning](http://semver.org) guidelines. Releases will be numbered with the following format: `<major>.<minor>.<patch>`


## Additional Information
For additional information, visit the Spunky Bot website at [https://www.spunkybot.de](https://www.spunkybot.de).

If you have any questions about Spunky Bot or need help, please use the [mailing list](https://groups.google.com/group/spunkybot) or post the question on our [forum](http://forum.spunkybot.de). If you need help right now, you can also find us on [Twitter](https://twitter.com/spunkybot).

In our [Google+ community](https://plus.google.com/communities/116728939500870368885) we talk about anything our community is interested in.

If you have bug reports or feature suggestions, please use the [issue tracker](https://github.com/SpunkyBot/spunkybot/issues?state=open).


## Contributing
You can help us in different ways:

* Open an [issue](https://github.com/SpunkyBot/spunkybot/issues) with suggestions for improvements
* Fork this repository and submit a pull request
* Improve the [documentation](https://github.com/SpunkyBot/spunkybot-docs) (separate repository)

By contributing code to this project in any form, including sending a pull request via GitHub, a code fragment or patch via mail or public discussion groups, you agree to release your code under the terms of the MIT license that you can find in the [LICENSE](https://github.com/SpunkyBot/spunkybot/blob/master/LICENSE) file included in this source distribution.


## License
The code of Spunky Bot is released under the MIT License. See the [LICENSE](https://github.com/SpunkyBot/spunkybot/blob/master/LICENSE) file for the full license text.


### Third Party Libraries
 - RCON: [pyquake3.py](https://github.com/urthub/pyquake3)
	- The library has been modified to fix some error handling issues and fulfill the PEP8 conformance. This file is released under the GNU General Public License.
 - GeoIP: [pygeoip.py](https://github.com/urthub/pygeoip)
	- The library has been extended with the list `GeoIP_country_name` to support full country names (e.g. Germany for country_code DE). This file is released under the MIT License.
 - Schedule: [schedule.py](https://github.com/dbader/schedule)
	- This file is released under the MIT License. 

Urban Terror™ and FrozenSand™ are trademarks of 0870760 B.C. Ltd.