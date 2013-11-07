RPi-Xively-Tutorial-Python
======================

Since the tutorial provided by xively didnt exactly work out of the box, here is the version that I was able to get to work
<br>
Here is the location of the Xively Tutorial, https://xively.com/dev/tutorials/pi/


1. Install Python Libraries
This version of code requires Python2.7 for xively to function correctly. It does not work with Python3.2 and I have not checked Python 3.3.

There is a dependency on the external "requests" Python library that has to be installed first

<pre class="code-text-only" style="display: none;">
<code><b># Xively Library Installation </b>
git clone https://github.com/kennethreitz/requests
git clone https://github.com/xively/xively-python
cd xively-python
ln -s ../requests/requests

<b># verify import throws no errors</b>
echo "import xively" | python2.7</code>
</pre>

2. Run the python script
<pre class="code-text-only" style="display: none;">
<code>sudo python2.7 xively_tutorial.py</code>
</pre>
