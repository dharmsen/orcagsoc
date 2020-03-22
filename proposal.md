[LICENSE](https://github.com/orcasound/orcagsoc/blob/instructions/GUIDE_LICENSE.md) (This template was adapted from [ESIP](https://www.esipfed.org/)'s organization [template](https://github.com/ESIPFed/gsoc/blob/master/STUDENT-proposal-template.md): thank you ESIP!)

#  Orca Location Detection Using Multilateration with Hydrophones

## Abstract

Short description of your project. Max 10 sentences. This **SHOULD NOT** be a
copy of the project idea text.
Whenever an Orca is near the hydrophones placed by OrcaSound and makes a sound, this can be picked up by hydrophones. This alone will not suffice to pinpoint the location of the killer whale, since we cannot derive the distance from just a single signal. By using 3 microphones, we could use a triangulation algorithm to pinpoint the approximate location of the orca when making the noise using the time difference of arrival of the signal between the three microphones. This feature can have future developments in a mapping with sounds, or researchers can be notified upon detection and be able to know the approximate location of the killer whale.  

## Technical Details

Long description of the project. **Must** include all technical details of the
project, like libraries involved.
By using three hydrophones set up at a reasonable distance from eachother, it should be possible to derive the distance between the location of the source of a call signal and the location of the microphones. It should also be possible to derive an estimated location of the source. We find this data using [multilateration and TDoA](https://en.wikipedia.org/wiki/Multilateration). Solving a system of equations with [3 microphones](https://www.canal-u.tv/video/inria/using_more_than_two_microphones.33283) and their respective timestamps would give an approximate location based on an intersection between two hyperboloids. 

Since accurate timestamps of detection are crucial to deriving a good approximation of the location, timestamps from the start of a detection based on for example the "Active Listening and Learning of Orca Sounds" idea would not suffice. Instead, we could calculate the phase difference between difference signals to derive the TDoA.

To implement the algorithm fully, it would be possible to use the [Google Maps API](https://developers.google.com/maps/documentation) to place the microphones and to get the location of the source signal. Solving the equation can be done using various libraries, but to be specific I will use the [numpy linear algebra library](https://docs.scipy.org/doc/numpy/reference/routines.linalg.html).

Difficulties that could arise during the project are for example the absence of an actual system implemented in real life now. This can be solved by making the algorithm based on a model system and evaluating capabilities based on this. Furthermore, the difference of temperature of the water, among other factors, can contribute to inaccurate findings. It could be possible to make a flexible system based on for example temperature data, but I am not sure whether this would yield good improvement. 

Here it is also important to document previous conversations with your prospective mentors. You can show relevant pieces of code that you want to change. You can link to literature you used during the research.

### Contributions So Far
This is my first time contributing to Orcasound and my first proposal attempt. If there would be a change, I will change this.  

## Schedule of Deliverables

Here should provide a list of your milestones. Below are a series of suggested sub-sections based on the
different phases of GSoC. You can use it as a template, but you can/should add more details
for each phase, e.g. by breaking it down into weeks or setting specific targets for each
phase. Each target should be split into sub-tasks with time estimates. [Work
breakdown structures](https://en.wikipedia.org/wiki/Work_breakdown_structure) may be helpful here.

### **Community Bonding Period**

This phase is to get to know the community better. Check that your build environment is setup. This time should also be used to discuss your project in more detail with the community, including introducing yourself and beginning to vet your ideas. 

*Note:* We require you to write regular blog posts. Now is a good time to become familiar with blogging in Wordpress, or let us know you already know how to use it. If you are accepted, we will provide you with an account on the Orcasound blog.

In this period I would set up a Wordpress and make sure it works correctly. Furthermore I would look into the technical details: how would my system be able to work with what is at hand? Communication between the organisation is vital in this part, since it would pave the road for the weeks ahead. If there are also people who are working with the orcadata projects listed in the ideas document, it would be nice to communicate between them to find out how we can intertwine our projects. Communicating with people working on the orcamap projects could also be interesting, considering the data retrieved from the system could be fed to an interactive map.

### **Phase 1**

Deliver a model that is accurate, realistic and works.

### **Phase 2**

Deliver a working implementation, hopefully ready for deployment.

### **Final Week**

At this stage you should finish up your project and ensure that you have code submitted to your organization. Our main criteria to define your project as a success is submission of code advancements before the end of GSoC.
Evaluate the deployed implementation, fix any errors that could rise up.

## Development Experience

Do you have code on github? Can you show previous contributions to other projects?
Did you do other code-related projects or university courses?
I have code on github, however incomplete. 
The past academic year I've studied Computer Science & Engineering at the [Eindhoven University of Technology](https://www.tue.nl/en/), but the year before I studied Data Science at the same university. I still follow some Data Science project courses. So far we have done projects about analyzing airline Twitter data, Diabetic Retinopathy detection with medical eye images, and supermarket data for optimal pricing.


## Other Experiences


## Why this project?

Apart from hearing the sounds orcas make, it might also be interesting to see *where* the sounds come from. The location data could be an interactive map with clickable sounds. Furthermore, the implementation of the algorithm could be very useful for researchers, who, as mentioned before, can be notified of locations. If the orca heard sends out a distress signal, this can be crucial information for finding out where to orca is in order to investigate what is wrong. Apart from the serious implications, it can also be used to spot the orcas in the area for educational or leisure purposes. The project also fits in with the other orcadata projects which, when combined, could make a very cool automatic location-deriving system. As for personal motivation, I am deeply saddend by the decrease in biodiversity that has been happening for the past few decades. I would like to contribute to the relief of this problem. Orcas, among other sealife creatures, are beautiful and should not be allowed to go extinct.
