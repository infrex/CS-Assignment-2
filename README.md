# CS Assignment 2
## Questions for TAs
- Should we have a "master" diagram that showcases the whole system?
    - A: We should have a master (high level) diagram, which describes the whole system
- Using JWTs, how should we display our diagrams? Should there be a node called "JWT service", which gets visited every time something happens a user clicks uses any operation? Can that be implied? Shuold we instead focus on explaining how it works via text?
    - A: Make an abstract node and explain the magic behind it
- Regarding database, do you have any tips/recomendations? Should we have one database or many databases for different things such as different microservices or for example one for pictures and one for passwords etc.?
    - A: Read the book "Security in computing" chapter. Common mistakeis to be missing DMBS. The core of it is that you isolate the parts of the DB, simple operations might mess up the whole DB. Handling access (who gets to access certain parts) is crucial. Everyone that wants to talk to the database should talk though the DBMS (gateway service (analogy))
- What should the focus be for the person responsible for the server? Should it be connecting all the different components such as the modem, router and printers or should it rather focus on the different microservices such as Book management system and such.
    - A: Focus on software
- Should use cases be blackbox or whitebox? Do we need to explain the innerworkings or the system?
    - A: Do not introduce any new information only what has already been explained in the document. Do not make too many, at least one. You could make one for each system, but it's not mandatory. Focus on blackbox, no options for correct option, wrong option ectc... USE CASE SCENARIO, not use case
## Extras
- Describe what hash algorithm you use (SHA256 recomended), write a paragraph about it, write what algorithms we considered (whirlpool) and write why we chose SHA256
- DBMS - implement this
- Different user roles, how do you control what users can access what stuff. Its very important
