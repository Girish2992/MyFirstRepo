# eCAL Foxglove Bridge

## Dataflow of the eCAL Foxglove Bridge

-  The ecal_live bridge will subscribe to all available Protobuf channels.
-  ecal_live will forward the respective data to the websocket interface of Foxglove-Studio.

## Build the eCAL Foxglove Bridge

- The eCAL Foxglove bridge can be obtained from the original [repository](https://github-am.geo.conti.de/ecal/ecal-foxglove-bridge).
```
git clone git@github-am.geo.conti.de:ecal/ecal-foxglove-bridge.git
```

- Install the needed requirements and the eCAL wheel for the eCAL version you want to build the eCAL Foxglove Bridge with
```
pip install -r requirements.txt
pip install /path/to/ecal-wheel.whl
```

- The executable can be created using the following Pyinstaller command:
```
pyinstaller ./ecal-foxglove-bridge.py --onefile
```
