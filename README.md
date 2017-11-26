# deSEC snap - DRAFT

This simple snap updates the configured deSEC domain names every five
minutes. Configure it by providing your token:

    $ snap set desec-idontgit password=<secret>

And configure your domain name list (comma-separated, no spaces):

    $ snap set desec-idontgit username=domain1.com,domain2.com

That's it. The daemon runs every five minutes. Check the journal for output,
including any problems:

    $ sudo journalctl -u snap.desec-idontgit.desec.service
