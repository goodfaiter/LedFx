=====================================================
   Welcome to LedFx ✨ *Making music come alive!*
=====================================================
|Build Status| |License| |Build Status Docs| |Discord|
|Contributor Covenant|

.. image:: https://raw.githubusercontent.com/LedFx/LedFx/main/ledfx_assets/banner.png

What is LedFx?
----------------
LedFx makes your LEDs dance to audio!
What LedFx offers is the ability to take audio input, and instantaneously processes the audio into realtime light show to multiple LED strips/matrix.
No need to spend hours on end to program one song to program your LEDs, as LedFx will do this all for you!

LedFx real-time LED strip music visualization effect controller using is a network based devices (ESP8266/ESP32/Raspberry Pi 4) with support for advanced real-time audio effects! LedFx can control multiple devices and works great with cheap ESP8266/ESP32 nodes allowing for cost effective synchronized effects across your entire house!

Demos
-------

Visit and join our `Discord`_ where community members show off their projects. Check out the #projects or #show-and-tell channels.

📑 Quick start guide and documentation📖
------------------------------------------

Head over to `releases`_ to get the latest releases for Windows and Mac. For linux, use pip.

**Bleeding edge (Experimental)**

If you want the absolute bleeding edge and are not afraid of using the terminal, take a look at the detailed installation instructions here: `Installation documentation`_.

**Documentation**

Documentation for the latest release can be found here: `Stable documentation`_

Documentation built against this repository can be found here: `Latest documentation`_


😍 Show me how to make one!
-----------------------------

The below image describes a basic setup - LedFx running on PC, communicating with a WLED Device controlling an LED strip.

.. image:: https://raw.githubusercontent.com/LedFx/LedFx/main/docs/_static/topology.png

.. list-table::
   :widths: 75 75
   :header-rows: 1

   * - Component
     - Example
   * - Computer running LedFx
     - Windows 10, `LedFx.exe`_
   * - Networked device controlling LED Strip
     - ESP8266 NODEMCU v3 running `WLED`_
   * - Addressable LED strip
     - DC5V WS2812B 5 meters 60LED/m IP67
   * - Power supply for LED Strip and ESP
     - 5V 10 amps LED Power Supply
   * - Something to connect the wires together!
     - Soldering iron/solder

#. **Build your networked LED Strip.**
      - For most, this is the difficult step. Don't worry! There's guides here and online, and plenty of people able to help on WLED and LedFx Discord.
      - Follow the `WLED guide to connect the LED strip and ESP together <https://kno.wled.ge/basics/getting-started/>`_.
      - `Flash WLED to the ESP device <https://kno.wled.ge/basics/install-binary/>`_.
      - Ensure all WLED devices are powered on, and connected to your Wi-Fi.
      - Test you can access the WLED web interface from your PC. If so, then you're good to go!

#. **Install LedFx.**
      - For PC and Mac, see our `releases`_, or see the `installation documentation`_ for more information.
      - For linux, you can use pip to install ledfx - however you may need to install some dependencies first. See the `installation documentation`_ for more information.

#. **Direct computer audio output to LedFx.**
      - By default on Windows LedFx will attempt to listen to your system audio.
      - More information for `Linux and macOS users here <https://ledfx.readthedocs.io/en/latest/directing_audio.html>`_.
      - Play some music in the background.

#. **Start LedFx.**
      - Your WLED devices should appear in LedFx, automagically configured and ready to go! 🎆🔥
      - If not, on the bottom click Home,  -> ``Scan for WLED devices`` button, or click on the big plus sign and ``Add Device`` to add them manually.
      - If they're still not showing up, make sure they're powered on and properly connected to your WiFi.

#. **Start using effects!**
      - Click on the device, select an effect eg ``scroll`` under Classic
      - Your lights should now be reacting realtime to your music! Enjoy the show 🌈


🧑‍💻 Join the LedFx Community
------------------------------

Join the Discord server to discuss everything about LedFx!  |Discord|

To join, click on the Discord button below:

.. image:: https://discordapp.com/api/guilds/469985374052286474/widget.png?style=banner2
   :width: 30%
   :target: https://discord.com/invite/xyyHEquZKQ

Contributing
--------------
Pull requests are welcome. Once tested, contact LedFx developer community on Discord to discuss the next step.
We expect and require all contributors to read, understand and follow our code of conduct.

Credits: `Contributors-&-About`_

License
---------
`GPL-3`_


.. _`GPL-3`: https://choosealicense.com/licenses/gpl-3.0/
.. _`LedFx.exe`: https://github.com/LedFx/LedFx/releases/latest
.. _`LedFx Guide`: https://ledfx.readthedocs.io/en/latest/index.html
.. _`WLED`: https://kno.wled.ge
.. _`releases`: https://github.com/LedFx/LedFx/releases/latest
.. _`Installation documentation`: https://ledfx.readthedocs.io/en/latest/installing.html
.. _`Stable documentation`: https://ledfx.readthedocs.io/en/stable/
.. _`Latest documentation`: https://ledfx.readthedocs.io/en/latest/
.. _`our website`: https://ledfx.app
.. _`Discord`: https://discord.gg/xyyHEquZKQ
.. _`Contributors-&-About`: https://ledfx.app/about/
.. _`How to: Enable Stereo Mix in Windows 10`: https://thegeekpage.com/stereo-mix/


.. |Build Status| image:: https://github.com/LedFx/LedFx/actions/workflows/ci-build.yml/badge.svg
   :target: https://github.com/LedFx/LedFx/actions/workflows/ci-build.yml
   :alt: Build Status
.. |Build Status Docs| image:: https://readthedocs.org/projects/ledfx/badge/?version=main
   :target: https://ledfx.readthedocs.io/
   :alt: Documentation Status
.. |License| image:: https://img.shields.io/badge/license-GPL3-blue.svg
   :alt: License
.. |Discord| image:: https://img.shields.io/badge/chat-on%20discord-7289da.svg
   :target: https://discord.gg/xyyHEquZKQ
   :alt: Discord
.. |Contributor Covenant| image:: https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg
   :target: CODE_OF_CONDUCT.md
