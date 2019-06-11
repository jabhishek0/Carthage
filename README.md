# Carthage installation guide


1:Install HomeBrew \n
2:Download and run the Carthage.pkg file for the latest release> https://github.com/Carthage/Carthage/releases \n
3:MacPorts \n
4:Clone from source and run make install

After installing Carthage
cd to project ${path} and type 
#touch Cartfile
it creates a Cartfile
now type
open Xcode -a Cartfile
this opens the Cartfile from Xcode
copy github "SwiftyJSON/SwiftyJSON" in Cartfile
save and exit the Cartfile
Now use
carthage update 
it will start downloading the SwiftyJSON in your project repo
in terminal type open Carthage 
drag and drop the SwiftyJson.framework from builds folder to Xcode>General>Linked Frameworks and Libraries
Select Build Phases 
Click on "+" Select New Run Script
Select "+" on input files and enter $(SRCROOT)/Carthage/Build/iOS/SwiftyJSON.framework
Now under shell enter the follwing commands /usr/local/bin/carthage copy-frameworks

Now press Command+B to build the app and test if set up was done succefully


