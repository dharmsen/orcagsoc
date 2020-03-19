[LICENSE](https://github.com/orcasound/orcagsoc/blob/instructions/GUIDE_LICENSE.md) (This template was adapted from [ESIP](https://www.esipfed.org/)'s organization [template](https://github.com/ESIPFed/gsoc/blob/master/STUDENT-proposal-template.md): thank you ESIP!)

#  Orca Location Detection using Trilateration

## Abstract

Short description of your project. Max 10 sentences. This **SHOULD NOT** be a
copy of the project idea text.
Whenever an Orca is near the hydrophones placed by OrcaSound and makes a sound, this can be picked up by hydrophones. This alone will not suffice to pinpoint the location of the killer whale, since we cannot derive the distance from just a single signal. By using intervals between two or more near microphones, we should be able to derive the distance based on the speed of sound in salt water. Using three of these setups, we could use a triangulation algorithm to pinpoint the approximate location of the orca when making the noise. This can have future developments in a mapping with sounds, or researchers can be notified upon detection and be able to know the approximate location of the killer whale.  

## Technical Details

Long description of the project. **Must** include all technical details of the
project, like libraries involved.
By using two near hydrophones, it is possible to 

Here it is also important to document previous conversations with your prospective mentors. You can show relevant pieces of code that you want to change. You can link to literature you used during the research.

### Contributions So Far
Write a subsection which lists your contributions so far to Orcasound or the project. This may include:
* Issues, PRs
* Resources Review
* Preliminary Attempts
Provide links whenever possible.

## Schedule of Deliverables

Here should provide a list of your milestones. Below are a series of suggested sub-sections based on the
different phases of GSoC. You can use it as a template, but you can/should add more details
for each phase, e.g. by breaking it down into weeks or setting specific targets for each
phase. Each target should be split into sub-tasks with time estimates. [Work
breakdown structures](https://en.wikipedia.org/wiki/Work_breakdown_structure) may be helpful here.

### **Community Bonding Period**

This phase is to get to know the community better. Check that your build environment is setup. This time should also be used to discuss your project in more detail with the community, including introducing yourself and beginning to vet your ideas. 

*Note:* We require you to write regular blog posts. Now is a good time to become familiar with blogging in Wordpress, or let us know you already know how to use it. If you are accepted, we will provide you with an account on the Orcasound blog.

### **Phase 1**

Deliverables

### **Phase 2**

Deliverables

### **Final Week**

At this stage you should finish up your project and ensure that you have code submitted to your organization. Our main criteria to define your project as a success is submission of code advancements before the end of GSoC.

## Development Experience

Do you have code on github? Can you show previous contributions to other projects?
Did you do other code-related projects or university courses?
I have code on github, however incomplete. 
The past schoolyear I've studied Computer Science, but the year before I studied Data Science at the same university. I still follow some Data Science project courses. So far we have done projects about analyzing airline Twitter data, Diabetic Retinopathy detection with medical eye images, and supermarket data for optimal pricing.


## Other Experiences


## Why this project?

Apart from hearing the sounds orcas make, it might also be interesting to see *where* the sounds come from. The location data could be an interactive map with clickable sounds. Furthermore, the implementation of the algorithm could be very useful for researchers, who, as mentioned before, can be notified of locations. If the orca heard sends out a distress signal, this can be crucial information for finding out where to orca is in order to investigate what is wrong. Apart from the serious implications, it can also be used to spot the orcas in the area for educational or leisure purposes. 
