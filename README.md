# earthdata-login-jupyter
A script that spawns a simple and secure widget for authenticating with NASA Earthdata in Jupyter environment.

### Run the script like an import all:
![prompt](docs/prompt.PNG)
### Password is entered securely with Python's `getpass` module
![prompt](docs/prompt.PNG)
### Successful login:
![prompt](docs/prompt.PNG)
### Successful login:
![prompt](docs/prompt.PNG)


![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
*Simple text login prompt.*

[ursjupyter.py](ursjupyter.py) is just a widgetized version of the **Python 3** authentication example (that uses the `requests` module) given at this link:
https://wiki.earthdata.nasa.gov/display/EL/How+To+Access+Data+With+Python

Passwords are entered securely and aren't retained after the session inits. There is one hack-y piece; authentication is tested against an ORNL DAAC Daymet granule (just a few KB), so that granule's download statistics are artificially inflated no doubt. Looking for suggestions on an alternative to that.