# Running a Python Script in Google Colab

This repository contains a Python script that can be run in Google Colab. The script automates the setup of a development environment for building Android APKs using Kivy and Buildozer.

## Usage

Follow these steps to run the provided Python script in Google Colab:

1. **Clone or Download Repository:**
   - Clone or download this repository to your local machine.

2. **Upload to Google Colab:**
   - Upload the repository to your Google Colab environment. You can do this using the "Files" tab on the left or by using the `!wget` or `!curl` commands to fetch files from the web.

3. **Run the Python Script:**
   - Open a code cell in your Colab notebook and run the provided Python script by executing the following commands:

   ```python
   !rm -rf sample_data/
   !pip install buildozer
   !pip install cython
   !sudo apt install -y git zip unzip openjdk-17-jdk python3-pip autoconf libtool pkg-config zlib1g-dev libncurses5-dev libncursesw5-dev libtinfo5 cmake libffi-dev libssl-dev
   !pip3 install --upgrade Cython==0.29.33 virtualenv
   !pip install kivymd kivy pymongo
   !sudo apt-get install -y python3-pip build-essential git python3 python3-dev ffmpeg libsdl2-dev libsdl2-image-dev libsdl2-mixer-dev libsdl2-ttf-dev libportmidi-dev libswscale-dev libavformat-dev libavcodec-dev zlib1g-dev
   !pip install python-for-android
   !sudo apt-get install -y libgstreamer1.0 gstreamer1.0-plugins-base gstreamer1.0-plugins-good
   !sudo apt-get install libffi7 build-essential libsqlite3-dev sqlite3 bzip2 libbz2-dev zlib1g-dev libssl-dev openssl libgdbm-dev libgdbm-compat-dev liblzma-dev libreadline-dev libncursesw5-dev libffi-dev uuid-dev
   !sudo apt-get install build-essential python-dev
   !sudo apt-get install build-essential libsqlite3-dev sqlite3 bzip2 libbz2-dev zlib1g-dev libssl-dev openssl libgdbm-dev libgdbm-compat-dev liblzma-dev libreadline-dev libncursesw5-dev libffi-dev uuid-dev libffi7
   !sudo apt-get install libffi-dev
   !yes | buildozer android clean
   !yes | buildozer init
   !yes | buildozer -v android debug


View Script Output:
As the script runs, follow the output in the Colab notebook to ensure that each step completes successfully.


That's it! You've successfully set up the development environment and built an Android APK with debugging enabled in Google Colab.
