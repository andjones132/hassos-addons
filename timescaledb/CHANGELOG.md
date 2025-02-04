# 2.0.0
 
!! READ CAREFULLY - Breaking changes !!

Upgraded PostgreSQL to 14.2 🎉
Upgraded TimescaleDb to 2.6.0 🥳
Upgraded Postgis to 3.2.1 👍🏻
Upgraded pgAgent to 4.2.2
Upgraded base images to 11.1.1
It took a while before this release came out. Covid came (and went!), but more importantly: Timescale 2.0 came out, just as PostgreSql 13 and 14.
I know that a lot of you guys (and girls) were waiting for support of Timescale 2+, but I had to be very careful not to break your existing setups.

The goals was to bring a seamless upgrade experience for both Timescale, Postgis, as well as Postgresql itself.
To perform these upgrades all together was not trivial, but, it's here!!

Please read the link below carefully to thoroughly understand the new breaking changes in TimescaleDb.

(see: https://docs.timescale.com/timescaledb/latest/overview/release-notes/changes-in-timescaledb-2/)

May you find any issues during install and/or upgrade, please open an issue on Github: https://github.com/Expaso/hassos-addon-timescaledb/issues

Thanks for all your support!

# 1.1.6

- Added armhf architechture
- Added max_connection configuration-option to set the maximum number of connection PostgreSql will accept.

# 1.1.5

- Added armv7 support: Closes #7 Add armv7 compatibility. Thanks to @berga (#8)

# 1.1.4

- Upgraded Postgres to 12.4 (see: https://www.postgresql.org/docs/12/release-12-4.html)
- Upgraded TimescaleDb to 1.7.4 (see: https://github.com/timescale/timescaledb/releases/tag/1.7.4)
- Added possibility to use system_packages:[str] and init_commands:[str] in your config, to further customize the container during startup.

# 1.1.3

- Upgraded TimeScaleDb to 1.7.2 (see: https://github.com/timescale/timescaledb/releases/tag/1.7.2).
- Fix problem whereby permissions on data-directory are wrong after snapshot restore.

# 1.1.2

- Prevent add-on exit when pgAgent-extension cannot be installed correctly.

# 1.1.1

- Support for more versions of TimecaleDb. This is needed when upgrading existing installations.

# 1.1.0

- Upgraded TimeScaleDb to 1.7.1 due to critical issues in 1.7.0 (see: https://github.com/timescale/timescaledb/releases/tag/1.7.1)
- Added pgAdmin extension

# 1.0.3

- Fixed error during CREATE EXTENSION IF NOT EXISTS postgis CASCADE

# 1.0.2

- Fixed error during add-on startup on Rpi3 and Rpi4

# 1.0.1

- Temporary version without TimeScaleDB Tuning

# 1.0.0

- Initial release
