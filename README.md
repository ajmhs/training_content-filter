# Console application based on Shapes which displays use of content filtered topics

Skeleton created via
 
`rtiddsgen -language C++11 -platform x64Linux4gcc7.3.0 -example x64Linux4gcc7.3.0 -create makefiles -create typefiles -d c++11 shapes.idl`

The publisher sends a "sine wave" pattern of orange squares, one every 30ms. Since the topic name is "Square", RTI Shapes Demo can also be used to publish data in different colours. 

The subscriber uses ncurses to display the different sample values in colour and has a log buffer in the last 15 lines which shows the current status of the content filter.

The content filter starts at y >= 0 AND y <= 50 and moves down by 10 pixels every 10 seconds. Once the filter window hits the bottom of the available Shapes Demo space, the filter is reset to the starting values.
