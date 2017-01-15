Install and Setup

0. Install Firefox in the default location
1. Make sure you have Python 2.7 or above installed on your computer.
2. cd splinter && sudo python setup.py install
3. cd ../openpyxl && sudo python setup.py install
4. download https://github.com/mozilla/geckodriver/releases and place in system PATH (/usr/local/bin on Unix)

Running:

1. sudo python iBuy.py username password file [line]
	- username and password are your iBuy username (w/o @uic.edu) and password
	- file is the .xlsx file containing the purchase order (other extensions should work but are untested)
	- [line] is the line number of the first item you would like the script to add (default 8)
		- this is only useful for purchase orders containing multiple vendors
		- the script will scan downwards starting at the line specified until it encounters an item from a different vendor
2. Enter your computer's password
3. You will be logged in to iBuy in a new Firefox browser window.
4. Enter the Supplier in iBuy when prompted to by the script.
5. Switch back to the terminal and hit enter.
6. After execution, verify that the information has been copied successfully before submitting the order.