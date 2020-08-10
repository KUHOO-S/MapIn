# MapIn
## DevJams 2019 

## Table of Contents
* [Ideology](#ideology)
  * [Work Plan](#work-plan)
* [Getting Started](#getting-started)
  * [System Requirements](#system-requirements)
  * [Installation](#installation)
* [Working Video](#working-video)
* [References](#references)
<!--ideology-->
## Ideology:
Several technologies have emerged that help people to navigate outdoors, but none of them work accurately when it comes to navigation inside a building for example. This causes problems when one is trying to find a room inside a building.
We are proposing to build an app to help users navigate indoors without going through the hassle of buying and fitting external hardware or worry about internet connectivity issues. We propose to use the technology of AR mapping by using the AR Core Library and Android studio to build an app for Indoor Navigation.

### Work plan
The problem of creating the "AR" map is solved by using an approach similar to that used
by Google Street View. During the one-time mapping process for every building, the AR
library would create 3-D pictures at various locations in the building.
The algorithm to find out where the person is present at any point in time is through the
following sequence:
1. We assume that we know the initial position of the user in the building.
2. The current guess is based on the current image we see through the user's camera.
3. Let's say the user moves and now we find a new image from the camera. The newly
obtained image is then matched with the 3-D images collected for that building. The
current image obtained from the camera is compared with the 3-D images, starting from
the current guess, adding the current velocity vector, and moving farther in circles.
4. Now, when the 'difference' in the images is below a certain threshold, we find a match!
We continue the same procedure to keep finding the user’s current location.

## Getting Started

### System Requirements:
#### ARCore Library requires: (https://developers.google.com/ar)
* Android 7.0 or later (some models require newer versions as noted below)
* A device that originally shipped with the Google Play Store
* Internet access, in order to install or update Google Play Services for AR
#### Android Studio requires:(https://developer.android.com/studio)
* Microsoft Windows 7/8/10 (32-bit or 64-bit)
* 3 GB RAM minimum, 8 GB RAM recommended (plus 1 GB for the Android Emulator)
* 2 GB of available disk space minimum, 4 GB recommended (500 MB for IDE plus 1.5 GB for Android SDK and emulator system image)
1280 x 800 minimum screen resolution.

### Installation

1. Clone the repo
```sh
git clone https://github.com/KUHOO-S/MapIn.git
cd BroBot
```
2. Open Android Studio and Build

## Working Video:
https://drive.google.com/file/d/1qQFQ8YqTHYQUwsRAz4XIXahOdMaw8WGM/view?usp=sharing

## References

1. [1]https://developers.google.com/ar
1. [2]https://www.favendo.com/wayfinding/what-is-indoor-navigation
1. [3]https://www.microsoft.com/en-us/research/blog/path-guide-new-approach-indoor-navigation/
1. [4] Curran, Kevin; Furey, Eoghan; Lunney, Tom; Santos, Jose; Woods, Derek; McCaughey, Aiden (2011). "An Evaluation of Indoor Location Determination Technologies". Journal of Location Based Services. 5 (2): 61–78.
1. [5] Chiou, Y; Wang, C; Yeh, S (2010). "An adaptive location estimator using tracking algorithms for indoor WLANs". Wireless Networks. 16 (7): 1987–2012.
