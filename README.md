# Kingst LA1010 support for Sigrok

To enable Kingst LA-1010 support in libsigrok there need perform these steps:<br>
<ol>
  <li>get libsigrok sources (see docs for libsigrok);</li>
  <li>copy directory 'kingst-la1010' to subdirectory 'src/hardware' in libsigrok source directory;</li>
  <li>apply patches 'Makefile.am.patch' and 'configure.ac.patch' to corresponding files in libsigrok source directory;</li>
  <li>build libsigrok (see docs for libsigrok);</li>
  <li>use Python script 'sigrok-fwextract-kingstvis.py' for extracting firmwares from 'LA1010.dll'</li>
  <li>copy firmwares to directory '~/.local/share/sigrok-firmware/'.</li>
</ol>
Extracting firmwares is avalible from KingsVIS executable which are provided with new version of Kingst software for Linux platform (tested on version 3.4.1).
