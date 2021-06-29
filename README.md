# dogo
dogo is a simple python3 program to dump mongodb database all in one go

# what does dogo do

By default all the mongodb instances are not protected by any username and password with such instances open to the internet attackers can dump the database to steal sensitive information and might possbily even gain unauthorized access to the infrastructure.

**mongo-db instances can often reveal some critical information such as target-OS target-arch and even what programs are installed, This can save time spent in fingerprinting and help us craft more precise attacks**


# Running and Installing dogo

*dogo runs on python3 so python3 should be installed on your system Below is the List of libraries you may need to install using pip3*

        $ pip3 install pymongo
        $ pip3 install termcolor
        
*once done with this you can clone the repository and run dogo*

        $ git clone https://github.com/SxNade/dogo
        $ cd dogo
        $ chmod +x dogo
        
        $ ./dogo <target-ip> <target-port>


![run](https://github.com/SxNade/SxNade.github.io/blob/main/dogo(1).gif)

# Searching mongo-db instances

**you can search for possibly open mongodb instances present all over the internet on services like shodan**

*This is a simple Shodan Query for mongodb on shodan: https://www.shodan.io/search?query=mongodb*

*Not all instances of mongodb you will find are open, some instances might be password protected , in that case we can try bruteforcing the password , there is a nmap NSE script for this purpose:: https://nmap.org/nsedoc/scripts/mongodb-brute.html *

**very soon a python script to bruteforce mongodb will also be released as part of this repo**

![shodan](https://github.com/SxNade/dogo/blob/main/mongodb.png)
