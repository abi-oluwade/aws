# Task
We want to be know how to launch an AWS instance, and then with that instance be able to install our Sparta nodejs app as well as
the mongodb, run a provision script to install the libraries and dependencies on that AMW instance, replace the default sites-enabled nginx with the nginx.default that we modified ,and then be able to launch the app so that it can be navigated to though the public ip.

This means we have to know commands below such as the scp command which can copy local folders and files to our AWS instance, which computers are located elsewhere.

- Port 22 is the SSH connection.

- ./<script or file name> runs the file

- scp -i ~/.ssh/Abiodun-Oluwade-Eng48-first-key.pem -r environment/ ubuntu@34.255.198.62:/home/ubuntu/ (command to copy entire folders to another machine, in this example copy environment to my AWS machine)

- scp -i ~/.ssh/Abiodun-Oluwade-Eng48-first-key.pem app/provision.sh ubuntu@34.255.198.62:/home/ubuntu/provision_file.sh (command to copy a single file folder)
