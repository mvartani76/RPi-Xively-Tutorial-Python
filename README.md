RPi-Xively-Tutorial-Python
======================

Since the tutorial provided by xively didnt exactly work out of the box, here is the version that I was able to get to work
<br>
Here is the location of the Xively Tutorial, https://xively.com/dev/tutorials/pi/

<ol>
<li><b>Create Xively Account</b></li>
You will need to go to https://xively.com/get_started/ and follow the links to create your account.

<li><b>Git xively tutorial source code</b></li>
<pre class="code-text-only" style="display: none;">
<code>git clone https://github.com/mvartani76/RPi-Xively-Tutorial-Python</code></pre>

<li><b>Navigate to newly created directory<b></li>
The previous step will download the code to <b>./RPi-Xively-Tutorial-Python/</b>. Navigate to this directory.
<pre class="code-text-only" style="display: none;">
<code>cd RPi-Tutorial-Python</code></pre>

<li><b>Install Xively Python Libraries</b></li>
This version of code requires Python2.7 for xively to function correctly. It does not work with Python3.2 and I have not checked Python 3.3.

There is also a dependency on the external "requests" Python library that has to be installed first.

<pre class="code-text-only" style="display: none;">
<code><b># Xively Library Installation </b>
git clone https://github.com/kennethreitz/requests
git clone https://github.com/xively/xively-python
cd xively-python
ln -s ../requests/requests

<b># verify import throws no errors</b>
echo "import xively" | python2.7</code>
</pre>

<li><b>Update FEED_ID and API_KEY</b></li>
Each device has unique information. The provided code uses the FEED_ID and API_KEY for my RPi using my Xively account.<br>

Change the following lines of code in <b>xively_tutorial.py</b>. You will need to navigate back to the <b>/RPi-Xively-Tutorial-Python/</b> directory.
<pre class="code-text-only" style="display: none;">
<code>FEED_ID = "2090009607"
API_KEY = "djUHb7PVHKYMlvxJn4gbAmtX2wC4SAniAniNHzm8QxexHyxW"</code></pre>
to
<pre class="code-text-only" style="display: none;">
<code>FEED_ID = "YOUR FEED ID"
API_KEY = "YOUR API KEY"</code></pre>

<li><b>Run the python script</b></li>
<pre class="code-text-only" style="display: none;">
<code>python2.7 xively_tutorial.py</code>
</pre>
</ol>
