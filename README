README Biabam 0.9.7                                          Dec 02 2004

Biabam Is A Bash Attachment Mailer

To use BIABAM use the following syntax (yes, it is on my todo list, to add
switches so the syntax get's like mailing with commandline Mutt):

echo <body> | biabam <attachment1,attachment2,attachmentN> -s <subject> \
 <recipient1,recipient2,recipientN>

Example:
echo "Here are the tarballs you requested" | \
  biabam foobar-0.7.8.tar.gz,coolapp-0.4.3.tar.gz,otherapp-4.3.0.tar.gz \
 -s "Answer to your request" john@doe.org,irene@prima.org,cira@alpispa.es

Other example:
$ echo "Take a look at these files" | biabam /mnt/cdrom/readme.txt,tux.png \
 tropical@premium.com

If no text is piped into biabam, it will wait for text on standard input
(finish with CTRL-D)

 By default, the comma ',' character is the separator for attachments and
 recipients, but you can customize this at the beginning of the script in a
 variable named SP.

TIPS:
 - Dont use the ; character as separator if you are calling biabam manually
   from an interactive shell because bash interprets it as command separator.
 - Dont use filenames with blank spaces unless you know your quoting
 - Dont use paths like ~/filename or ../filename
 - The separator can be more than one character length(e.g. '%%%').

IMPORTANT:
In order to use BIABAM you need the uuencode utility, because the script relies
on it to do base64 encoding.
BIABAM also requires sendmail or equivalent MTA installed on the system,(for
example qmail has a sendmail wrapper). If your MTA is not /usr/sbin/sendmail
you will have to change the variable SENDMAIL and SENDMAIL_OPTS in the
beginning of the biabam file.

AUTHOR

  Mads Martin Jørgensen <mmj@mmj.dk>

RELEASE MANAGER

  Frederik Juul Christiani <frederik@christiani.dk>

ACKNOWLEDGEMENTS

  Thanks to:
  Roman Drahtmüller <draht@suse.de>
  Stefan Reinauer <stepan@suse.de>
  Thomas von Elling Skifter Eibner <thomas@stderr.net>
  Douglas Johnston <dougj@pendragon.bristolgroup.ca>
  Morten Poulsen <mortenp@certus.dk>
  Nathan Hurst <njh@hawthorn.csse.monash.edu.au>
  Bastian Kleineidam <reflexionsniveau@web.de>
  Nelson Benitez <gnelson@inMail.sk>

  For advice, additions and good company ;-))
