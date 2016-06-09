# hw10-final-proj-documentation
Link to word file of this (https://www.dropbox.com/s/fv8wm2i02vwxu2d/18.%20N_Smith.Final%20Proj_Final%20Documentation.docx?dl=0)

Nathaniel Smith
Professor 
Class
6/9/16

Programming Final Project Documentation 
“Analog Pixel Mirror: Flippy, Move When I Move and When I don’t”


i.	Project Summary Status: At the moment the board remains wired up according to the initial documentation called for by the flip dot manufacturer. This includes the connection between the Arduino Uno, RS 485 breakout and finally the Flip Dot (7X7) Matrix Board. The camera aspect of the board has not been fully integrated as of yet. It was kept out of the testing for the purposes of isolation to the system testing. An animation sequence was designed and to the best of my ability I coding the placeholders of the flip dots. I was then attempting to get the Flop Dot matrix to perform to discern the logic of the board to finalize the code. Testing of the device was as success in that it is clear that information is accurately coming into the Arduino and moving through the RS 485 to the flip dot board. This confirmed the wiring is correct. However, the tests were not successful in getting the flip dot board to perform data based operations per the code that was written. This documentation then serves as a snap shot in time of the project, not a final documentation of the project.

ii.	Future Work to Be Addressed: 

    a)	Reach Out to Flip Manufacturer: Due to the fact I was unsuccessful in getting the board to perform operations based on code. I am going to be providing accurate documentation to the mfg. of all the work that has been done to show that my board is in fact wired up correctly. It tests accurate and all the pixels work, but it is not performing. 

    b)	Acquire Sample Code: My hope is that the reach out will result in getting some sample code and perhaps a correct configuration for that code to the device. This hopefully will include DVP settings, Dip Switch address and some code that will work with Arduino and push through the RS 485 breakout they suggested. 

    c)	Following The Success of My Project: After I am able to get the board to work accurately I plan to make a much more clear visual guide for people to be able to create projects with the flip dot boards more easily then it has been for me. There are some gaps in how to do a great many things between the wiring and coding and I hope to bridge that gap for future makers. 


iii.	Process-Project Research: I scoured the world looking at everyone else who had done projects using this technology. I cataloged all of the examples. I read through their code. I sourced my parts. All of the research that I did for this project is very well labeled and linked to this RTF document. 

    a)	Link to Research: (https://www.dropbox.com/s/3v13di7q62fmk0w/4. Research For Final Project.rtf?dl=0)


iv.	Process-Step One Project Write Up: I wrote a thorough examination of what the project would purport to be. It included an executive summary description that covered a system architecture description, inputs, outputs, data description, visual example, and my original inspiration. I covered the components and parts, the challenges I thought I would face and a milestone break for a project timeline. 

 a)	Link to Initial Write Up: (https://www.dropbox.com/s/988tbrneknhkxvk/5. Smith.N_P%26E_Final Proj_Analog Pixel Mirror.docx?dl=0)


v.	Process-Step Two [Components] Sourcing Parts: 

    a)	64 led pixel matrix board: I acquired this from the hybrid lab to get started and start experimentations while I waited for my flip dots to ship in. 

    b)	Flip Dots: I spent a good amount of time going back and forth with the manufacturer on what board they had in stock that was small I could learn from and how soon I could get it. They are in Poland so I had to do all my communicating with them mostly after midnight, as that was firs thing in their morning. Finally we decided on the board I  

    c)	Ada Fruit Camera From Jame Co: I ordered this camera, which appears to be the best one on the market to work with arduino from JameCo for ease of speed. It has great documentation too, which made it an easy choice. 

    d)	All Prototyping Lab Materials: I knew that I was going to have to build this project mostly after school was out so I bought everything that the hybrid lab offers so I could end to end produce the project in my own studio. The only thing I didn’t buy was a 3D printer as it isn’t a necessity for my lab and I have access to many others. However I got everything else soldering gun, octopus extra hands, jump wires, insulation lines, steel wool cleaner, heat gun and all hand tools. 

    e)	RS-485: I didn’t realize I needed the RS-485 board until I actually got started building and it was very last minute. I realized when I started to dig in that I would need to communicate through that to actually talk to the board, so I quickly bought this at the end of my work. 

vi.	Process-Step Three Build Prototyping Lab In House: All of my components arrived with the lab components. Naturally I build the lab before I started to assemble my project so I could have all the tools at the ready for the make. This proved to be very valuable as it gave me no limitations to waiting on a tool to be available to me or access to my project. I am incredibly excited I must say for the future as well to have the start of a solid lab at my ready access. 


vii.	Process-Wire Up Board:

    a)	The flip dot mfg. had a solid layout of the board and how to wire it up.

    b)	I didn’t understand how to run the wires into the back of the flip dot matrix so I sought assistance from prof. Michael Shiloh, who was able to guide me through that layout. 

    c)	Once I had the flip dot board powered and wired up I needed to route everything to the RS-485. This proved to be a bit difficult as it called for me to run 3.5V and RTS together and into the arduino 3.3 v. I didn’t know how to run two wires together to go into one pin so I didn’t do it at first. Then when my board wouldn’t work later I figured this aspect out. Only to still not have the dummy code run.


viii.	Process-Source Code:

    a)	I sourced as good of code libraries I could find on the web. I have listed those in my research. I also have iterations of them in my git hub repository of the work I did on them.
    
    b)	I still could not get the dummy code to run on the board after tearing through the documentation. 


ix.	Process-Test Animation Sequences for Flipdot Board:

    a)	64 led pixel matrix board: I started with this board while I was waiting for the flip dots to ship in. I was able to get the board to work very easily and build out my animation sequence to run on it. However this was a back up plan and not my actual plan, so it wasn’t very meaningful other then to the flip board work.

    b)	I designed and laid out one graphical explanation of an animation sequence I hoped to code and run on the flip dot display. I put the code I believe to be assigned to each dot in place so that once I was able to establish communication with the board I could write code to make it work.
    
    c)	I was never ever to establish communication.

d)	The document I laid out for the animation is here: (https://www.dropbox.com/s/qjmmtbqw5iiusan/Flip Dot Run Sequence %231 Outy Inny_V 2.pdf?dl=0)


x.	Process-Debug Flipdot Board: 

    a)	Flip Dot Documentation Addresses & Dip Switch: I combed through the documentation and found the right settings for the physical buttons on the back of the board. 

    b)	Wiring: I double-checked all of my wiring according to the schematic that was given by flop dot. 

    c)	Code: I walked through at length all of the libraries I was using to see if I could find the correct settings others had been successful with.

    d)	I had my engineering partner in Canada go over the project with me and look at it. We were both confused by the 60 data points in the code that were coming through the library as there were 4 assignment bytes that were necessary and 49 bytes that appeared to control the flip dots on the board. It was unclear then what was going wrong in the code.

xi.	Process-Present: My presentation process was during hacker hours and this ended up being a debugging session for the project. I walked through all the documentation I had assembled, code and my sequence. Nor prof. Shiloh, prof. Zamfirescu-Pereira or I could diagnose the problem. We tried making sure the board settings were correct. We looked at all the connections to make sure they were good. We pulled out the oscilloscope to see the flow of data through the board and it was in fact-moving data, but not in the way the board wanted somehow. We concluded the effort by manipulating and isolating the code libraries I put together, but that was not successful either. 

xii.	Conclusive Results: The conclusion that that what needed to happen was for me to get the camera working and moving information in the system eventually and to reach out the flip dot mfg. In the interim I would put together a comprehensive documentation for the project. 

