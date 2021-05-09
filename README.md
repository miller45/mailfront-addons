This is a copy-mod-hack from the original (see forked from header).
Changes I made:
- Excluded files from Makefile that I could not fix
- Fixed these to compile with mailfront-2.22 i.e. newer version of bglibs:
  backend-qmailsump plugin-dcc plugin-greylist.so plugin-chkdns.so plugin-authres.so
- Adapted the Makefile.local to build in its own directory
  You have to set MAILFRONTPATH to your local mailfront src dir


These are additional plugin modules for Bruce Guenther's mailfront
SMTP daemon, updated for mailfront 2.00.

You need the mailfront software first, which you can get here:

http://untroubled.org/mailfront/

For the authres and arlog plugins, you need SPF and DKIM and DMARC libraries.

libspf2 is from http://www.libspf2.org/

libopendkim is from http://www.opendkim.org/

Both have linux packages and FreeBSD ports available.  I've only built
them with the FreeBSD ports.

libopendmarc is at http://sourceforge.net/projects/opendmarc/


