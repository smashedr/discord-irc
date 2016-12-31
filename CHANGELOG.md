# Changelog
This project adheres to [Semantic Versioning](http://semver.org/).

## [2.1.6] - 2016-12-08
### Fixed
* Listen to warn events from Discord.
* Listen to debug events from Discord (only in development).
* Log info events upon connection, instead of debug

## [2.1.5] - 2016-11-17
### Fixed
* Upgraded node-irc to 0.5.1, fixing #129.

## [2.1.4] - 2016-11-14
### Fixed
* Added support for highlighting users by their nicknames,
thanks to @DarkSpyro003.
* Upgraded to discord.js v10.

## [2.1.3] - 2016-11-02
### Fixed
* Send text messages only to text channels (thanks @dustinlacewell).

## [2.1.2] - 2016-11-01
### Fixed
* Use nickname, not username, in command prelude.
Thanks to @williamjacksn.

## [2.1.1] - 2016-10-21
### Fixed
* A bug where Discord attachment URLs weren't posted to IRC, thanks to @LordAlderaan for the report.

## [2.1.0] - 2016-10-09
### Added
* Messages sent to IRC will now use the correct server nickname,
instead of the user's global username (thanks to @DarkSpyro003).

## [2.0.2] - 2016-10-02
### Fixed
- Display custom emojis correctly, thanks to @macdja38.

## [2.0.0] - 2016-09-25
### Fixed
- Upgrade to version 9.3 of discord.js.
This removes support for Node.js versions older than v6,
as that's the oldest discord.js supports.

## [1.0.3] - 2016-09-09
### Fixed
- Replace changes in 1.0.2 with the #indev-old version
of discord.js.

## [1.0.2] - 2016-09-09
### Fixed
- Discord's API now requires bot tokens
to be prefixed with "Bot". This adds
a hotfix that does exactly that.

## [1.0.1] - 2016-06-19
### Fixed
- Upgraded dependencies.

## [1.0.0] - 2016-05-06
### Changed
- Breaking: discord-irc now uses tokens for authentication, instead of
email/password, thanks to @TheDoctorsLife. See the README for more instructions.

## [0.8.2] - 2016-04-21
### Fixed
- Enable auto reconnect for IRC and Discord.

## [0.8.1] - 2016-04-21
### Fixed
- Upgrade discord.js to 7.0.1.

## [0.8.0] - 2016-04-04
Implemented by @rce:
### Added
- Support for messages containing both attachments and text.

### Changed
- Attachment URLs are now posted by themselves, instead of including a
preliminary message explaining that it's an attachment.

## [0.7.0] - 2016-04-04
### Added
- Added the config option `ircNickColor` to make it possible to
disable nick colors for messages sent to IRC.

## [0.6.1] - 2016-04-04
### Fixed
- Upgrade dependencies.

## [0.6.0] - 2016-02-24
### Added
- Highlight Discord users when they're mentioned on IRC (thanks to @rce).

## [0.5.0] - 2016-02-08
### Added
- Discord attachments will be linked to on IRC when
they're posted (fixed by @rce).

## [0.4.3] - 2016-01-23
### Fixed
- Upgraded dependencies.
- istanbul -> nyc for coverage.

## [0.4.1] - 2015-12-22
### Changed
- Comments are now stripped from JSON configs before they're parsed.
- Upgraded dependencies.

## [0.4.0] - 2015-11-11
### Added
- Colors to IRC nicks.

## [0.3.0] - 2015-10-28
### Changed
- Rewrote everything to ES6.

## [0.2.0] - 2015-10-28
### Added
- Support for channel and username highlights from Discord to IRC.
This means that e.g. #general will no longer result in something like #512312.

### Added
- Working tests for all functionality.

## [0.1.1] - 2015-10-27
### Changed
- Made `discord.irc` a regular dependency, instead of a devDependency.

## [0.1.0] - 2015-10-13
### Added
- Initial implementation.
