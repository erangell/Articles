# dZeZ : thoughts about open source ZZ data structures for the decentralized internet

## Background
Ted Nelson has patented and trademarked ZigZag&reg; for development of his zippered-list constructs.  See https://xanadu.com/zigzag/ for more information.  dZeZ is an exploration of how ZZ data structures may be implemented as a data access layer in a decentralized web environment.

## Definitions (provided by Ted Nelson):
- zzspace is the arbitrary space of cells connectable
  arbitrarily plus to minus in a plurality of dimensions

- a zzstructure is anything built in this space

- a zzengine, like Gzz,
  has operations upon zzstructure,
  and views so that you can see what you're doing.

- Recommended reading: https://xanadu.com/zigzag/ZZdnld/zzRefDef/

## What is dZeZ?  
- dZeZ aims to be an open source conceptual data structure that represents graph data structures using technologies available on the decentralized web.  zzstructure is a special case of a graph that imposes a restriction (known as "Restriction R") on how cells may be connected ( see https://eprints.soton.ac.uk/259230/1/mSpace_zzStructures.pdf  )
- A graph contained in a dZeZ data structure may be validated to verify compliance with restriction R
- Tools for building dZeZ data structures may choose to enforce Restriction R to ensure that mutations of the graph always comply with Restriction R, and can take advantage of features specific to zzstructures.
-  While dZeZ will initially take advantage of features of a specific dWeb protocol (hypercore protocol and its derivatives: https://hypercore-protocol.org ), the concept is intended to be a protocol-agnostic abstraction layer that can wrap any decentralized data technology that conforms to a dZeZ interface.

## How do you pronounce it?
- You have a choice: Dee Zez (an homage to Zez Confrey) or Dee Zee Easy.

## Main features of the Decentralized Internet: 
- Append-only logs get replicated across peers who subscribe to them or seed them for others.
- The data access protocol may have built in versioning and peer discovery, and abstracts the
network connectivity via APIs
- Each item of data on the decentralized network is content-addressable using a hash that is verified by a merkle-tree structure (a distributed hash table, such as a Kademlia DHT).  This eliminiates the need for addressing by server, user, or URL.  The same content can be served by any node on the network that chooses to seed it, which is the equivalent of a transclusion of the source material.
- Protocols may allow for sparse access to blocks of data using index structures.  Applications can also design custom access methods.

## Features of Decentralized Web Applications
- Many custom applications can be developed against the same data structures, tailored to the needs of the user community, or even individual users.
- Applications can be configured to run in an offline environment, disconnected from the internet, accessing local copies of data previously retrieved from the network.

## The Vision
- Open source communities can develop decentralized applications outside of corporate boundaries.  Users should always have a choice to take their data with them as they migrate to different applications.
- Users can either contribute their own storage and bandwidth resources to the network or participate in communities which pool resources and use smart contracts to enforce proper behavior of nodes which serve the community.  ( see https://playproject.io/ )
- Ted Nelson's book: Literary Machines (https://en.wikipedia.org/wiki/Literary_Machines ) describes his vision for a docuverse where all connections between documents are available and visualized in various views.  Many of the conceptual structures described in that book can be upcycled. 
- While the semantic web offers several data formats (ex: RDF, JSON-LD), zzstructures 
should be available as another choice for applications.  Such structures can be implemented at different abstraction levels.  For example, a hyperdrive can use directories to implement tumbler addressing. ( see https://en.wikipedia.org/wiki/Tumbler_(Project_Xanadu) )
- Enfilades ( see https://en.wikipedia.org/wiki/Enfilade_(Xanadu) ) can be used as indexing structures for hypercores or hyperdrives, and shared across the network.
- Rich Links connect spans of content with a tagging system of user-defined types.  They use tumbler addressing, which can be extended into the dweb space.
- Edit-decision-lists can be maintained by authors and readers, and fulfilled via peer-to-peer connections.
- Transcopyright can be implemented by adding end-to-end encryption within webs of trust on top of the data published on the network.
- Front end applications can build upon the functionality demonstrated in the Gzz prototype, and ideas demonstrated in the other prototypes of zzstructure.  The idea would be to simplify certain operations so they make sense to the user.  For example, auto-cloning could be done behind the scenes to preserve compliance with Restriction R.  Hints of available connected dimensions may also be useful for user contextual orientation.
- Multiple views of either generic graph structures or zzstructures can be built in either marketplaces or open-source communities.
- Note that IP anonymity is external to decentralized protocols and requires additional components in the networking stack.  Encryption services are now provided by certain protocols.
- Hyperdrives have a "mount" feature which allows any other hyperdrive to be mounted as a subdirectory of a hyperdrive.  This feature essentially extends the tumbler addressing space for a given user/hyperdrive, allowing links to be created to that user's copy of another person's hyperdrive by using the tumblers in the mounted subdirectory.

## Versioning options for documents stored in hyperdrives:
The choice of versioning strategy depends on the use cases of the application.  Some alternatives are:
- use built-in versioning for files in a hyperdrive, referenced via URL
- transclude a full copy of every version from a git repo to a new tumbler
- keep full text of earliest version and maintain forward delta EDLs
- keep full text of latest version and maintain reverse delta EDLs


## Example
The “dzez” directory of this repository is an example of one way that directories of a hyperdrive could structured and used for tumbler addressing and zzstructure.  The readme.txt file in each directory is for comments about the contents of the directory and may be ignored by applications.  The example files will be revised over time as comments are received on this document.  The hyperdrive provides a way of tying all comments and discussions together in one place, by transcluding them from their original sources using a rich link that provides a way to navigate back to the sources. 

## Contributors
If you provide feedback on this document and agree to have your name listed as a contributor it will be listed here as you specify.

- Eric Rangell: Solutions Architect, Independent Contractor, Pennsylvania

