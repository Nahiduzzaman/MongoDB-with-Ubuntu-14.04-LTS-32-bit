Command #1:
>sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10

Command #2:
>echo "deb http://repo.mongodb.org/apt/ubuntu "$(lsb_release -sc)"/mongodb-org/3.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.0.list

Command #2:
>sudo apt-get update

if in the end this command provide this error:
>E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem.

Do this,
>cd /var/lib/dpkg/updates

>sudo rm *

And then run the below command to get newer ones,
>sudo apt-get update

Command #2:
Command #2:
Command #2:
