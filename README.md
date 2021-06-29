# dogo
dogo is a simple python3 program to dump mongodb database all in one go

# what does dogo do

By default all the mongodb instances are not protected by any username and password with such instances open to the internet attackers can dump the database to steal sensitive information and might possbily even gain unauthorized access to the infrastructure 

# Running and Installing dogo

*dogo runs on python3 so python3 should be installed on your system Below is the List of libraries you may need to install using pip3*

        $ pip3 install pymongo
        $ pip3 install termcolor
        
*once done with this you can clone the repository and run dogo*

        $ git clone https://github.com/SxNade/dogo
        $ cd dogo
        $ chmod +x dogo
        
        $ ./dogo <target-ip> <target-port>

