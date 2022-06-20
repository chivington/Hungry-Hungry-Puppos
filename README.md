<p align="center">
  <img width='350' src='https://github.com/chivington/Hungry-Hungry-Doggos/blob/main/imgs/hungry-hungry-puppos.png' alt='Hungry Hungry Puppo Logo'/>
</p>

# Hungry-Hungry-Doggos
A raspberry pi based pet feeder / treat dispenser of any small objects. It includes:

1. food dispenser
2. water dispenser
3. treat dispenser
4. door opener
5. dog's room camera

I created this automation system because I am working 12 hr days and wanted to be able to feed Mullis and let him out during the day. Currently, the camera feed and treat dispenser are operational. Contact me by email to find out how to access the camera feed and feed him a treat.

The hardware and code are in place to operate the door opening system, but I'm printing worm gears because the motors are salvaged from cordless power tools to save money and make the system more reproducible. Instead of buying high torque motors, which are very expensive, a gearing system will enable the use of cheap, low torque motors to open & close the deadbolt and door.

<br/>
The system consists of:

1. An Nginx server that serves the main app
2. A Motion server that serves the camera feed
3. A Sanic server that serves the controls UI
4. The combination UI/state management Unity framework I created (See [Unity](https://github.com/chivington/Unity) for details)

Nginx serves the main app and proxies to the other servers for the camera feed and controls UI, which are embedded in the main app. Sanic is chosen for the controls due to it's asynchronous nature, which allows me to call controls subroutines without tying up threads.

![Build Status](https://img.shields.io/badge/build-Stable-green.svg)
![License](https://img.shields.io/badge/license-NONE-lime.svg)
<br/><br/><br/>

## Contents
* [Prerequisites](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#prerequisites)
* [Installation](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#installation)
* [Usage](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#usage)
* [Authors](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#authors)
* [Contributing](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#contributing)
* [Acknowledgments](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#acknowledgments)
* [License](https://github.com/chivington/Hungry-Hungry-Doggos/tree/master#license)
<br/>

## Prerequisites
  * None
<br/><br/>


## Installation
```bash
  git clone https://github.com/chivington/Hungry-Hungry-Doggos.git
```
<br/>


## Usage
This repo is only meant for viewing. You can visit [chivington.casa:3000](https://chivington.casa:3000) to see Mullis in his room and feed him a treat.

Feel free to ask me questions on [GitHub](https://github.com/chivington)
<br/><br/>


## Authors
* **Johnathan Chivington:** [Web](https://chivington.net) or [GitHub](https://github.com/chivington)

## Contributing
Not currently accepting outside contributors, but feel free to use as you wish.

## License
There is currently no license associated with this content.
<br/><br/>
