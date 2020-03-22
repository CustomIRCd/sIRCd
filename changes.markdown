# sIRCd Changes

## Changes since Version 1.1.2

- [] - make m_cloaking an extension again

## Changes since Version 1.1.1

- [X] - Import the code from ircd-seven to show the oper name and server used
- [X] - Add config option to hide durations of temporary K/D-lines
- [X] - Improve WEBIRC's TLS handling
- [X] - Make the oper chghost restriction configurable
- [X] - add @ prefix to op-moderated (+u) messages

## Changes since Version 1.1.0

- [X] - Add option to immediately apply nick RESVs by FNC'ing
- [X] - Various Fixes
- [X] - Add support for multiple forms of blacklist queries using matches
- [X] - Updated sqlite3 to 3.12.0
- [X] - Fix memory leaks and clean up code a bit.
- [X] - Add mbedtls implementation
- [X] - Remove kline_delay config option
- [X] - Tidy up daemonisation

## Changes since Version 1.0.9-2

- [X] - Re-enable away-notify
- [X] - add support for IRCv3.2 userhost-in-names
- [X] - allow the CharAttrs table to be modified at runtime
- [X] - notify public users the OPER that killed the user

## Changes since Version 1.0.9-1

- [X] - Move m_locops module to extensions.
- [X] - Added usermode +O which will hide oper from /whois for non oper accounts
- [X] - Added module chm_insecure, which requires users to use SSL to join channels unless mode +U is set
- [X] - Move show_whois into core
- [X] - Remove unused modules/extensions
- [X] - Added --with-shared-sqlite option for low end vps and Raspberry Pi style boards (requires package libsqlite3-dev)
- [X] - Added datarootdir that was missing
- [X] - Allow exact PID file prefix to be specified
- [X] - Removed smallnet option as never used



## Changes since Version 1.0.9

- [X] - Added usermode +I which will hide idle from /whois output for non oper accounts
- [X] - Reinstated configuration option for the nick of the SASL agent
- [X] - Moved ip_cloaking to modules and renamed to m_cloak. Automatically loaded now
- [X] - Dix gnutls error with version 3+
- [X] - Update openSSL 
- [X] - Removed unused cloaking
- [X] - Show users the RESV reason
- [X] - Purged local channels (not really used)
- [X] - Hard coded chm_sslonly into the core
- [X] - Fixed extb_channel bug where if banned target channel has +s or +p set it wouldn't work
- [X] - Use NAMELEN instead of NICKLEN when accessing Client->name because it could in theory be a HOSTLEN length string.

## Changes since Version 1.0.7/8
 
- [X] - Add vhost for opers support, requiring opers to identify with nickserv firstly
- [X] - Remove zip linking support
- [X] - Fix Compile errors
- [X] - Removed oponlymsg and named staffonly (mode +m prevents none IRCops messaging you)
- [X] - Use sha-512 for SSL
- [X] - Remove DES support for mkpasswd
- [X] - Upgrade sqlite to 3.8.10
- [X] - Remove last update to m_sasl.c
- [X] - Added another cloaking module

## Changes since Version 1.0.5/6

- [X] Change who can set selected channel modes
- [X] Remove NOKICKOPER(Channel mode +M) from core and make a module
- [X] Allow self-devoicing (enbaled/disabled via config)
- [X] Moved selected extensions to modules   
- [X] Fix halfop permissions (Allow self-dehalfop)
- [X] Show a client's unique ID on connect & whois
- [X] Add static parts
- [X] Remove m_roleplay
- [X] Add sasl_usercloak
- [X] Added m_forcequit (Allows admins to /forcequit users remote/locally and IRCOP's locally only)
- [X] Added show_whois - usermode +W which will notify you when someone does a /whois on you
- [X] Added a idle time feature for IRCOPs, if Idle for longer than set time they'll be removed from /stats p (defaults: 2hours)
- [X] Added extb_hostmask - Hostmask extban type: bans all users matching a given hostmask
- [X] Reverted ip_cloaking module back to original state
