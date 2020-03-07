# warfork_ansible
A repo with my warfork server configuration. Just automating stuff

For Debian based servers only, for now.

Requirements:
git
ansible

Basically just do
apt install git ansible

And then use
ansible-pull -U https://github.com/babitz0r/warfork_ansible

This will automatically create a steam user, download steamcmd, install warfork and put in my custom config templates as well as add aliases so you can have commands for launching servers and updating warfork.
All that is left for someone to do is to manually edit the .cfg files to their liking and that's it.

The .cfg files are normal.cfg, insta.cfg, priv.cfg, duel1.cfg and duel2.cfg, They're in /home/steam/warfork/Warfork.app/Contents/Resources/basewf
All you really need to do is edit the names of the servers, it should be fairly self evident. Don't forget to add your operator (admin) password as well. From these you can also get an idea on how to create your own .cfg files.

You can find all the commands at the bottom of the /home/steam/.bashrc file. Obviously you will need to log in as the steam user, so just do "su steam" if you're logged in as root. To simplify it:
wfsall - will run 5 servers, two of which are for duels, one is private, one is instagib with all gamemodes votabe, one is with normal weapons with all gamemodes votable
wfupdate - will update the game

With a bit of common sense + trial and error you can easily tweak everything to your liking.

If you need any help setting up your WF server(s), you can find me in the game's official discord or just message Babitz#4571
