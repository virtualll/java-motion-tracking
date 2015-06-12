## Overview ##
Tracks a virtually unlimited number of moving objects simultaneously, in a live webcam or prerecorded video, giving each object's current bounding rectangle coordinates, pixel count, etc., for each moment in time (each video frame). Possible applications include surveillance, pranks, interactive games, monitoring, traffic analysis. Start out by [watching the demo video](https://www.youtube.com/watch?v=2aFDTZlR7DM)!

You can play with the example Swing application, or use the libraries in your own application. JMF is used for video input.

The algorithm processes each frame of video through multiple stages of image processing to determine what is background and what is foreground (moving objects). Objects are given their bounding rectangles, and a "label" (numeric ID) that can be tracked throughout multiple frames.

The libraries and application are Eclipse Plug-In projects, but if there is enough demand for these to be regular Java or maven projects, I can convert them. So if you want/need them converted just let me know.

## Installing and Running ##
This project requires you to have installed:
  1. A 32-bit [Java Runtime Environment (JRE)](http://www.oracle.com/technetwork/java/javase/downloads/index.html) or JDK
    * A 64-bit JRE will not work because JMF (see next step) does not run on a 64-bit JRE.
    * To be able to run the .bat files in the bin folder on Windows, the 32-bit JRE must be your default JRE (the one in your PATH variable). If you haven't installed another JRE don't worry about that.
  1. The [Java Media Framework (JMF)](http://www.oracle.com/technetwork/java/javasebusiness/downloads/java-archive-downloads-java-client-419417.html#7372-jmf-2.1.1e-oth-JPR)

On Windows you can run the example application right away by going to the "bin" folder and running the .bat file of your choice there.