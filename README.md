RPi-Xively-Tutorial-Python
======================

Since the tutorial provided by xively didnt exactly work out of the box, here is the version that I was able to get to work
<br>
Here is the location of the Xively Tutorial, https://xively.com/dev/tutorials/pi/


This version of code requires Python2.7 for xively to function correctly. It does not work with Python3.2 and I have not checked Python 3.3.


# Xively Library Installation 
git clone https://github.com/kennethreitz/requests
git clone https://github.com/xively/xively-python
cd xively-python
ln -s ../requests/requests

# verify import throws no errors
echo "import xively" | python2.7
