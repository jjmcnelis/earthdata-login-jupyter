# earthdata-login-jupyter
A script that spawns a simple and secure widget for authenticating with NASA Earthdata in Jupyter environment.

[ursjupyter.py](ursjupyter.py) is just a widgetized version of the **Python 3** authentication example (that uses the `requests` module) given at this link:
https://wiki.earthdata.nasa.gov/display/EL/How+To+Access+Data+With+Python

Passwords are entered securely and aren't retained after the session inits. There is one hack-y piece; authentication is tested against an ORNL DAAC Daymet granule (just a few KB), so that granule's download statistics are artificially inflated no doubt. Looking for suggestions on an alternative to that.

------------------------------------------------------------------------------

![prompt](docs/prompt.PNG)               
*Run the authentication script like an import all.*

------------------------------------------------------------------------------

![password](docs/prompt2.PNG)                   
*Password entered securely with Python's `getpass` module.*

------------------------------------------------------------------------------

![prompt](docs/success.png)                     
*Successful login.*

------------------------------------------------------------------------------

![prompt](docs/fail.PNG)                         
*Failed login. Prompts repeatedly for new credentials; hangs Jupyter session until valid username and password are provided.*

------------------------------------------------------------------------------

