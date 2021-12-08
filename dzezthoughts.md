# dZeZ : thoughts about open source ZZ data structures for the decentralized internet

## Background
Ted Nelson has patented and trademarked ZigZag(R)&trade; for development of his zippered-list constructs.  See https://xanadu.com/zigzag/ for more information.  dZeZ is an exploration of how ZZ data structures may be implemented as a data access layer in a decentralized web environment.

## Definitions (provided by Ted Nelson):
- zzspace is the arbitrary space of cells connectable
  arbitrarily plus to minus in a plurality of dimensions

- a zzstructure is anything built in this space

- a zzengine, like Gzz,
  has operations upon zzstructure,
  and views so that you can see what you're doing.

## What is dZeZ?  
- dZeZ aims to be an open source conceptual data structure that represent graph data structures using technologies available on the decentralized web.  While it will take advantage of features of a specific protocol (hypercore protocol and its derivatives), the concept is intended to be a protocol-agnostic abstraction layer that can wrap any decentralized data technology that conforms to a dZeZ interface.

## How do you pronounce it?
- You have a choice: Dee Zez (an homage to Zez Confrey) or Dee Zee Easy.

## Initial Thoughts
I'm exploring how to create ZigZag data structures on the Decentralized Internet, 
where append-only logs would get replicated across peers who subscribe to them or seed them for others.
The protocol ( https://hypercore-protocol.org/ ) has built in versioning and peer discovery, and abstracts the
network connectivity via APIs, so people would be able to build many custom applications (most of which can
run in the browser) and they would share the same underlying ZZ data structures.

My reasoning is that while there are other data formats being used (ex: RDF, JSON-LD) Ted Nelson's ZZ structures
should be available for people to explore and build on as another choice for their applications.  So I am 
working it out in my mind and seeing pointers at the end of each hypercore referencing back to lumps of data
inside the core, and each core would be a dimension with a unique network address. 
Other cores would contain EDLs, Enfilades, Tumblers, and other index structures.
There will be seeding services to host the cores and keep them available without depending on domain ownership.  

In terms of the front end, I was playing with Gzz and thinking about how to use it for a simple problem:
Capturing transcripts and chats from Zoom meetings and creating rich links from the utterances and URLs.
It is difficult to get used to ZZ thinking, and the setup of data in Gzz is not intuitive.  Maybe if the UI had more
hints to guide users visually towards possible next steps and available dimensions it could be easier.
The process of thinking through this problem gives me insights about how the data structures would be constructed.


