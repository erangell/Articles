Opportunities for Decentralized Web Technologies in Education
===

by Eric Rangell

How can educators use emerging decentralized technologies to enhance educational experiences?  I am a software developer and solution architect, so I am not professionally qualified to answer that question.  However, I am also an out-of-the-box thinker, and have connected with a community (the [Digital Life Collective](https://diglife.com/)) that is enabling trusted digital collaboration across diverse communities, so I hope to make contributions towards long term goals that improve access, privacy, data portability, and verifiable recognition of student mastery.  Education has always been an interest of mine, while my career spanned software development for various industries since the 1990’s.  One unique project that I enjoyed was building a [remedial music theory course](https://diglifebeaker101.hashbase.io/rubric) for a university under the direction of two professors who met with me on weekends at a diner to discuss requirements and review deliverables.  I was able to deliver Java applets using MIDI which enabled student-driven exploration of each unit - the students were able to place notes on the staff and play them before they submitted their answers.  My knowledge of mainframe JCL inspired a PHP driven navigation through the course where each  Java applet could be called with different parameters depending on the material being taught.  I discussed the project on the [Ed-Tech Musician podcast](https://archive.org/download/WildKlezmerJazzManFreeCD/EricsInterviewOnEdTechMusician109.mp3) and that led to interest by an author writing an article in *Teaching Music* magazine, which was exploring Web 2.0 at the time.  Some people think we are in a Web 3.0 movement as the decentralization imperative grows legs.  I was inspired to explore it when Brewster Khale coined the phrase “[Lock The Web Open](http://brewster.kahle.org/2015/08/11/locking-the-web-open-a-call-for-a-distributed-web-2/)”, which means that the emerging decentralized technologies should ensure equal access, privacy, and prevent centralized control of information resources.  My exploration led to an interest in the [DAT project](https://datproject.org) and [Beaker Browser](https://beakerbrowser.com), and I connected with those communities.  I also became interested in the work of [Ted Nelson](https://www.youtube.com/watch?v=hMKy52Intac), [Douglas Engelbart ](http://dougengelbart.org/)and feel that decentralized technologies may soon enable practical implementations of their ideas.  I also explored the educational methods of [Richard Feynman](https://archive.org/details/ThePleasureOfFindingThingsOut_201809) and [Richard Hamming](https://www.youtube.com/watch?v=zA3-mLhajkk).  If you do not want to reinvent wheels and repeat historical mistakes, please stop reading this now and watch the linked video by Richard Hamming on Computer Aided Instruction: https://www.youtube.com/watch?v=zA3-mLhajkk

Before we even consider educational technologies, we need to understand our audience across several dimensions, some of which are: age, cultural environment, experience, learning styles, learning goals, special needs, and [neurotribes](http://stevesilberman.com/book/neurotribes/).  Consider how technology complements the learning experience of the audience, and whether individual tailoring of the material is necessary for specific people.  Learning styles are generally classifed as visual, auditory, and kinesthetic.  A learning path should provide the same material  in multiple formats that support each learning style.  Kinesthetic learners may need additional non-computer resources to provide tactile experiences of the learning material, which can be delivered as instructions for projects to build and discuss using audio/video media.  When working with students who exhibit extreme interest in specific topics it may be necessary to tailor the material in terms of their specific interests and encourage them to find their own paths for researching the subject.  It is possible that they may discover new ways of presenting material which can be incorporated into future versions of a class in a manner similar to a Github Pull Request (where a branch is developed and later merged into the main flow of a class).  Educators should also explore archives of online learning software, such as the [MECC series](https://archive.org/details/softwarelibrary_apple_mecc), and evaluate if any of them are practical for use in their courses.

My goals for any system that may be built from the ideas presented here are:
1. Encourage creativity while learning.
2. Develop a love for research.
3. Develop critical thinking skills, including the evaluation of sources of research material.
4. Improve personal time and knowledge management skills, and find creative ways to use downtime (such as listening to podcasts or watching educational videos).
5. Encourage collaboration with diverse communities.

Some of the advantages offered by decentralized web technologies are:

1. Privacy
2. Portability
3. Offline rich content experiences
4. Automatic versioning
5. Security built into the protocols

It is important for each technology to be transparent about any issues discovered, and to promptly address known vulnerabilities.  The objective is to develop trust to facilitate educator evaluation of the technology.  Educators need to define their threat model in terms of what controls. security, and audit features are needed to ensure successful operation of the selected technologies.  The objective is to create an environment of cooperation while reducing the need for competition.  Openness and open source are key to helping users understand and evaluate the technologies that may meet their needs.  Developers should welcome feedback from user communities and strive to improve their products over time by working in an agile manner with their stakeholders.

Let's take a deeper dive into the advantages of decentralized web technologies.

* Privacy

  Users are in full control of their work and what they choose to share with others.  This requires training in the features of the technology and an understanding of where their data resides at any given time.  Users also need to understand whether their data is encrypted at rest and in transit.  They need confidence that only the people they authorize can decrypt their work.  Certain scenarios may need additional controls, such as expiration of keys or time capsule locks.
  
  Decentralized systems are also working on solutions for identity managment that do not depend on passwords or corporate identity management.  The DAT project is investigating use of personal websites connected with user owned devices as a means for users to select among multiple identities for different scenarios ([DAT Identity proposal](https://www.datprotocol.com/deps/0006-session-data-extension/)).   Research has also been done on [self-sovereign identity](https://www.amazon.com/Comprehensive-Guide-Self-Sovereign-Identity-ebook/dp/B07Q3TXLDP), which uses open standards to establish user identity independent of corporate domains.  Educators need to understand that identity is a difficult problem and there will be a continuous need to upgrade security as additional threats emerge, however the technologies for good privacy and security exist now and will continue to improve.

  Another key feature that will become easier to implement over time is the creation of webs of trust, where groups can securely exchange confidential information over public networks that can only be decrypted by members of the web of trust.  Previously this required non-intuitive procedures to be followed by each user.  The built-in encryption features of decentralized technologies will make it easier to create these secure services.  
 
 * Portability
 
     Educators should ensure that their data is not locked in servers or databases that are proprietary or cannot be moved to other services.  Decentralized technologies are built with this consideration up front.  If similar services can operate on the same data formats, the user can test data portability while evaluating each service.  Open data formats are emerging such as [frictionless data](http://okfnlabs.org/projects/frictionless-data/).  Conferences such as [CSV,conf](https://csvconf.com/) can help you stay current.
 
* Offline Rich Content Experiences

  Decentralized protocols are agnostic to the transport layer, so Internet connectivity is not a requirement for applications to run.  Data synchronization operates on a policy of eventual consistency, and conflict-free replicated data types ([CRDTs](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)) are used when possible.  The student experience can include downloading of class content for offline review.  Students can make editable copies of this content and edit it for their purposes on their local machines.  To see an example of such an experience, visit: the following site in Beaker Browser: **dat://datbeakerroadmapnotes2018oct14.hashbase.io/**
  

* Automatic Versioning

  Decentralized protocols have been developed in a manner where all data is retained in append-only file structures.  This enables full traceability of changes and deletions of all versions of files or objects maintained in the archive.  Also, specific versions of code and data can be directly addressed using conventions in the URL.  A proposed enhancement to the DAT protocol known as [Mounts](https://github.com/datprotocol/DEPs/issues/32) will improve collaboration by virtually making another directory appear as a subdirectory of another DAT archive.
  
* Built-In Security
    
    Public key cryptography is fundamental to secure communications and transactions on untrusted networks.  The internal structure of DAT archives enables cryptographic verification of the content and its origin.  Therefore, a natural key exists that connects the user's machine to the content created.  Enhancements to the protocol using the open-source [Noise](http://www.noiseprotocol.org/) project will provide greater flexibility for applications to construct additional layers of encryption.  For education, the ability to easily create webs of trust with encryption at rest and in transit will be required in order to secure classes, content, and student records.
     
* Current state of decentralized technologies
    
    Education has traditionally been slow to change, and traditional institutions may have multi-year budgetary cycles which influence technology adoption.  Decentralized technologies are being explored by innovative communities and will need to mature before their value can be demonstrated in mainstream educational communities.  Visionary investors will fund pilot projects which advance research in this field.  I am putting forward a vision for a future where education is a personal individual journey that draws out the human potential of the student.  My pilot project is named "Climb DAT Mountain" and it needs educational stakeholders to work with the Digital Life Collective to clarify this vision and drive it forward, otherwise developers will build great tools that do not meet user needs.  Since I come from a software development background, I can only lead the agile development of the technologies to support the vision.
    
    I believe that enhancements in the following technical disciplines will be necessary to create the toolbox that instructors will use to create content for this project:
    
    1. User Identity needs to be standardized and proven.
    2. Multiwriter technologies need to be tested and simplified.
    3. Toolkits for web publishing need to be refined and simplified.
    4. Development frameworks need to support robust component models.
    5. The network needs to be stabilized and secure.

   Personlly, I have explored the Polymer lit-element framework for creating reusable React-like web components in an interative manner and have found the development experience enjoyable.  My work started after Paul Frazee published [this video](https://www.youtube.com/watch?v=m6zWt9fMkyE) which helped define a development framework.  Please visit [this Github repository](https://github.com/DigitalLifeCollective/ClimbDATMountain) for more information about Climb DAT Mountain use cases, and a simple prototype that uses components created in Polymer.

  I am refining my vision by participating in conversations about Open Learning and Personal Knowledge Ecology.  I continue to dream about how to bring the visions of Douglas Engelbart and Ted Nelson into practical use.  I will leave you with the following outline as a starting point for your dreams: 



    * Knowledge Ecology
        * Toolbox will be like a Github for course materials and designs.
        * Knowledge trails can validated by mentorship experiences.
        * Pull requests to enhance courses and learning paths.
    * Xanadu navigation
        * Explore Ted's vision, and current implementations.
        * Miller Columns may be sufficient as a starting point.
        * ZigZag data structure implemented with decentralized tech.
        * Explore code bases like [PushPin](https://github.com/inkandswitch/pushpin) (also see this [video](https://www.youtube.com/watch?v=hx3tnQNgGBc)) 
    * Transcopyright
        * Micropayments for works shared by publishers/
        * Cryptocurrency support, blockchain recordkeeping
        * Pay-as-you-go for material relevant to your reserach.
    * Mentoring Protocols
        * Informal mentorships between students completing the same course.
        * Formal mentorship arrangements, such as [this learning community](https://wtfsharp.net/wtf-is-fs-mentorship-program).
        * Social ledger credit for completed mentorships.
        * Redefine the concepts of Transcripts and Curriculum Vitae.    

If you are interested in working on the requirements, design, and testing of this project, please contact [Christina Bowen](https://twitter.com/csageland/).

If you are interested in the technical architecture, design, and coding for this project, please contact [Eric Rangell](https://twitter.com/RatifyArticle1).

