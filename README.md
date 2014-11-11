OpenCVBaseProjectXcode
======================
This is a simple OpenCV sample in xcode
to run this you should first install OpenCV from Brew

brew tap homebrew/science

brew install opencv

steps that i have done in Xcode 5:

Create a new Xcode project as OS X Application -> Command Line Tool, etc.
Click the target in the upper left
Click the Build Settings tab
Scroll down to (or search for) the Search Paths section
Under User Header Search Paths add /usr/local/Cellar/opencv/2.4.9/include
Click the Build Phases tab
Click Link Binary with Libraries
Choose the required libraries from /usr/local/Cellar/opencv/2.4.9/lib
At least, add libopencv_core.dylib
If you want pre-set command-line arguments, go to Product -> Scheme -> Edit Scheme (⌘<)
Click the Run tab on the left
Click the Arguments tab
Enter arguments into Arguments Passed on Launch
