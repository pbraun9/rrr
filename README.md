# Rogue Rolling Releases

_In case you're somehow unhappy with pkgsrc and slackbuilds_

I use this to build a few production daemons from source, so I am sure I get the latest version, whatever vendor's package is currently available for it.  Also note the main trick here is to link everything against the latest version of OpenSSL or LibreSSL into `/usr/local/`, no matter if the base system already has an older version of it.  Works best on NetBSD and Slackware Linux.

## Requirements

NetBSD sysprep --- In case you want to access to the GIT repo right from the start, you need to use pkgsrc anyway

	vi ~/.profile #enable PKG_PATH
	. ./.profile
	pkg_add -v git
	pkg_add -v mozilla-rootcerts
	pkg_add -v mozilla-rootcerts-openssl

Slackware sysprep --- Make sure some KSH is in Da Place

	ls -lF /var/log/packages/ksh93-*

## Usage

In example if you are missing Luke on Slackware  
 
        git clone https://github.com/pbraun9/rrr.git
        cd rrr/
        ./rrr lukemftpd

