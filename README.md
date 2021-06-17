# Global Address List OWA Extractor
*Allows extraction of the Global Address List (GAL) via Outlook Web Access.*

A request called `FindPeople` can be made that (with some small modifications) will allow you to get the entire Global Email Address List for your organisation.

In my testing, this script allowed me to get just under 5000 emails in about 5 seconds. As far as I know, this script only works with Exchange 2013 servers.

# Usage

The script can be run like so:
```

python emailextract.py -i webmail.example.com -u username -p password

```

Where the `-i` argument is the URL to the OWA landing page (do not include the `/owa` at the end), the `-u` argument is a valid username, and the `-p` argument is a valid password.


The discovered emails will be printed on screen, and also written to a file called `global_address_list.txt`. You can specify an alternate output file name with the `-o` argument.
