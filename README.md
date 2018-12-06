#### READ ME - Command-line client

Check for python version 3

`$python --version`  # Python 3.7.0

Install dependency

`$pip3 install requests`

At the command line, run:  

`$python3 client.py 3050107579885e1608e6fe50fae3f8d0 # Another example ID : 6681ac2f62509cfc220d78751b8dc524` 

You should see the following output printed in the terminal, for example: 

`Getting metadata for input sequence id : 3050107579885e1608e6fe50fae3f8d0 from https://www.ebi.ac.uk/ena/cram 

Success, status code is: 200
********************  METADATA  ********************
... ID: 3050107579885e1608e6fe50fae3f8d0
... LENGTH....... 7156
... TRUNC512..........  None
... ALIASES..........  []`

To print a JSON representation of the metadata returned, add this as an argument after the sequence ID, for example:
`$python client.py 3050107579885e1608e6fe50fae3f8d0 json`
 
The output will print the JSON object, for example: 
`{"metadata":{"id":"3050107579885e1608e6fe50fae3f8d0","md5":"3050107579885e1608e6fe50fae3f8d0","trunc512":null,"length":7156,"aliases":[]}}`

