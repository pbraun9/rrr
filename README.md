# Rogue Rolling Releases

Works best on NetBSD and Slackware Linux (in case you're somehow unhappy with pkgsrc and slackbuilds)

## Requirements

### NetBSD sysprep

In case you need access to the GIT repo right from the start, you need to use pkgsrc anyway

	vi ~/.profile #enable PKG_PATH
	. ./.profile
	pkg_add -v git
	pkg_add -v mozilla-rootcerts
	pkg_add -v mozilla-rootcerts-openssl

### Slackware sysprep

Make sure some KSH is in Da Place

	ls -lF /var/log/packages/ksh93-*

## Usage

In example if you are missing Luke on Slackware  
 
        git clone https://github.com/pbraun9/rrr.git
        cd rrr/
        ./rrr lukemftpd

