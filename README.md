# PTZCamSync

A simple application that allows users to manage [PTZ Optics](https://ptzoptics.com/) cameras and [OBS Studio](https://obsproject.com/) scene switching with a simple click of a button. This is a fork of [Column01](https://github.com/column01)'s program to get it to work with modern OBS Studio versions

## Setup

### Note

You can skip the python setup section by downloading the latest release of the program [here](https://github.com/sutterismine1/PTZCamSync-ModernOBS/releases)

If you'd like to play with the source directly, clone the repository to a folder you'd like to use for the program and follow along with all steps below.

### Setup Python Environment

1. Install Python 3.6+ 64bit
2. Create a python venv called "PTZCamSync" and activate it.
3. Run: `pip install -r requirements.txt` in this new command prompt to install all dependencies

### Configure OBS

OBS Studio 28.0.0 and newer includes obs-websocket out of the box so no additional plugin installation is required.
1. Create your scenes you wish to use and note their names down somewhere
2. Ensure the WebSocket server is enabled in the OBS Studio application by going to Tools > WebSocket Server Settings > Enable WebSocket Server
3. In the WebSocket Server Settings, make sure the Server Port is set to 4455 and that you have the server password by clicking Show Connect Info

### Configure PTZ Optics Camera

Follow your user manual on how to configure your PTZ Optics Camera and set presets. Make sure you note down the preset numbers for use later in configuring the program

### Configure the program

See the [configuration guide](CONFIGURATION.md) where it shows you how to configure your settings for the program. Note that the built-in WebSocket tool might give you a random password so make sure you follow the steps above and modify the password field in settings.json
