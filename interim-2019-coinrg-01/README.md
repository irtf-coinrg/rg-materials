interim meeting in June

Interim Meeting Recording
https://ietf.webex.com/recordingservice/sites/ietf/recording/playback/125e459bd3e84f28bb1f8a570fd53caa

agenda:
- review of the charter towards actualizing it
- Montreal hackaton
- Montreal meeting 
- other topics of interest

minutes:

COINRG - https://irtf.org/coinrg
Friday 07 June 2019
Interim meeting
Chairs: Jianfei (Jeffrey) He, Marie-José Montpetit, Eve M. Schooler
Meeting materials: https://datatracker.ietf.org/rg/coinrg/meetings/
-----
 
Attendees:
--------------
Aaron, Alex, CORE WG, Dave Oran (Network Systems Research & Design), Dirk Kutscher (University of Applied Sciences Emden/Lee), Dirk Trossen (InterDigital), David Lou, Daniel Bernier (Bell Canada), Emile, Eve Schooler (Intel), Ike Kunze (RWTH Aachen), Jianfei (Jeffrey) He (Huawei), Jörg Ott (Technische Universität München), Marc LeClerc (NoviFlow), Marie-Jose Montpetit (MIT), Ronald van der Pol (SURFnet), Xavier de Foy (InterDigital), Yvon Savaria (Polytechnique Montreal)
 
Agenda:
----------
- Review of the charter towards actualizing it
- Montreal P4 hackathon
- Montreal IETF 105 meeting 
- Other topics of interest
 
Charter
----------
MJM: Welcome to all. We have several folks from the P4 community, including those from Ecole Polytechnique and NoviFlow. And several newcomers.
The agenda today: discuss current charter, prepare for the upcoming P4 Hackathon (acknowledged as having a smaller scope than a COIN Hackathon), prepare for the upcoming COIN meeting.
Because we ran out of time at the last IETF, would like to focus the discussion here on the charter.
COIN proposes to look at everything that is programmable and  to advocate for richer programmability.
Its context is the Cloud-to-Edge continuum and the  evolution of the network from largely sending packets to combining networking with compute and storage.
High interest in what is currently underway with NetCache and Kubernetes, yet also very interested in use cases such as IIoT, AR/VR, autonomous/connected vehicles.
Need new architectures as well as functional distribution.
Paying close attention to DINRG and ICNRG (chairs from both are on the call), as well as interest in distributed networking (Dirk Trossen) and in the Transport area (Joerg Ott).
There is friction between E2E semantics of the network and E2E privacy/security, and COINRG ambitions to intercept some of the packets (an interest of Aaron Falk).
Decomposition of computational tasks is interesting, not just because of the Edge-ification of the Cloud that distributes parts of the computation, but also for energy efficiency.
 
Dirk K: Co-chair ICNRG and DINRG. Researching Networking and Distributed Systems.
One perspective to bring into the discussion: The list of topics in the scope includes programmable networks and devices.
However there are at least 2 things worthwhile to mention and to untangle.
Programmable networks, which could be perceived as using SDN for configuring and controlling the network and using languages like P4 to achieve (forwarding) behaviors for IP networks today.
The other aspect we haven't addressed sufficiently and certainly have not mentioned enough: networked computing, or distributed computing.
How could next generation distributed compute raise new requirements for networks and how could networks support them?
This could be the most interesting aspect of this group. Lots of distributed computing exists today in overlays in the cloud, but something new to look at: how could next generation distributed computing interact with the network, and how could the network support distributed computing from different research angles. What does it mean for protocols, security, manageability and also APIs? How would you actually work with this new capability and with this new kind of network?
 
MJM: Consider the aspect of mirroring: What can the network do for distributed compute and what can distributed compute do for networks? When we were looking at AI, a lot of people asked what can AI do for the network. Later, considered what can the network do for AI. Thus, raising the same kind of duality here.

Joerg Ott: [Happy Birthday! 2 days ago!]
Charter up to this point is written such that it could be interpreted or read in a number of different ways.  
Assumption however has always been: What can the network do for applications and not what the network can do for network management.
MJM: Absolutely.

Dirk K.: Why APIs are important is that it is always good to have a certain perspective on the implementation.

How can a research group enable real experiments that in some way evaluate these ideas?

May not need an extended list of milestones attached to the charter, but instead need a few first Goals.

What could COIN do to enable experimentation and validation?



[20:32-21:03 - audio outage]


Dirk T : When read the RG title, found it interesting it was called Computing in the Network. Reminded of a presentation given in a related effort in the ITU which is looking into Network 2030. Discussion in there on Edge computing.

Dirk has submitted a scenario on application level services as an I-D to COINRG.

Here, let’s discuss and question where the boundary of the network is, what is it that the network can bring to the task at hand?



MJM: The definition of the network is currently very fluid. This is why we are calling it a continuum.

But as a research group we need to focus and to scope.

Let’s move the editing of the charter to the mailing list.


Dirk T: A final comment on the charter: the use cases are geared toward requirements analysis. Identify what we are talking about and what we are NOT talking about, going forward. Requirements sounds too solutions/development oriented. 

MJM: There exists many Edge research efforts. We are looking for something original or unique, looking at research that is off the beaten path that is not being done elsewhere. 

P4 Hackathon

-----------------
MJM: The P4 language is dedicated to packet filtering at line speed. Has a C-like language. Done for speed. Doesn’t do floating point or multiplication, but does other cool things. We have experts on the call today.

Hackathon to happen 7/20-7/21. Remote participation will be possible. Will have multiple levels of people there. Beginners and experts. MJM falls in the middle; participated in a hackathon in Boston.

Marc to supply the group with the licenses and also will send us a few helpers.



Marc: Would like to tie the hackathon to the practical side.



Joerg: Caution that we should not let people misunderstand "COIN is exactly p4” or “COIN is only P4". What MJM liked around the Hackathons at the IETF, there are multiple WGs in the same room and cross fertilization. Acknowledged that this hackathon will be simpler and have a smaller scope than a COIN Hackathon.

Focused on P4, because there is a big P4 community in Montreal.



Marc: As a marketing person, sees a hackathon as having two objectives: 1) promote ideas and 2) attract people to participate in the execution of those ideas. Could call it a hackathon focused on a programmable forwarding plane.

However, need to make it interesting, yet the technology should not be too broad. In the case of Noviflow, we’ve been developing programmable forwarding planes for 7 years. We have a lot of experienced engineers who know how to use the Barefoot development tools. Therefore the hackathon could basically use Barefoot's toolkit to do the exercises. In contrast to what was done in Boson, have a suggestion on areas for things to look into. Example: take a look at the intimate connection between forwarding plane and application and services, e.g., ask the students to accurately test the latency of services, which would be a specific target so can be delivered within the scope of 2 days. Contrary to the Boston P4 hackathon, have more of a unified environment, have experts from NoviFlow provide assistance so they can focus on the idea creation, not on the tools.


MJM: Noa shared a link to tutorials, cheat sheets and basic P4 tools. Will share it to the mailing list. P4.org exists and is promoting the language.


Yvon: We have several students interested in using P4 for better network devices. Would like to have some of the students involved and help with this Hackathon.


Eve: In an Edge environment, marshalling resources and configuring those resources, marrying resource capabilities and job tasks, is all very complicated. How to scope down the space for a hackathon? Perhaps we think about a long term hackathon objective and break it down into smaller steps, over the course of several hackathons. Demonstrate a big hairy audacious goal, like some sort of smart city application. How to incrementally have hackathons that nibble on concepts in the space that demonstrate programmability and computation in the network. And their interplay with data management.



MJM: As Joerg noted, COIN is not about p4, there is a much bigger picture; a small piece of that picture is P4. Could use Montreal to define a bigger project. Will ask the list if there are specific project ideas for the Hackathon in mailing list. Will post P4 tools to the mailing list as well.

IETF 105 Montreal meeting

--------------------------------

MJM: 2 hours requested. COINRG was mostly successful in Prague, though didn’t have enough time to really discuss the charter. Need to look at and review the drafts, which include I-Ds from Dirk T, Eve, MJM, Jeffrey. Potentially a new draft on Industrial networks is in the works. Also someone from Chicago (new way to look at video distribution, a cool way of using computing in the network).



Ike: We are working on the industrial application draft. We are planning to be in Montreal, either me or my professor. We will try to submit the draft in time.


Dirk T: will be Montreal, if no conflict, will present my draft in person.

Jianfei: Dirk K mentioned in the mailing list that he may share some ideas about function placement and stateful computing.


Dirk K: Let me think about how I’d package and frame these ideas.

