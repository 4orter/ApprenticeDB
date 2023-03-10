# Demonstrate knowledge of key computer programming fundamentals

### Demonstrate an understanding of the history of computing

Computing as seen today is the result of hundreds of years of invention and research. Before there were any electronic computers, the term *Computer* referred to a person that calculated numbers or did arithmetic mentally using mathematical formula. Over the millennia, humans would create computing devices like the Abacus (Sumeria), the Astrolabe (Greece), the Difference Engine (Charles Babbage), the Tabulating Machine (Herman Hollerith), and the ENIAC (University of Pennsylvania) to make computing more efficient and less error prone. The invention of mechanical computers would eventually give rise to professions like "Computer Programmer" and "Computer Technician." Early computer programmers like Ada Lovelace typically wrote algorithms that solved mathematic and/or scientific problems. These algorithms or instructions would come to be known as "software." As innovation in computing hardware was giving rise to smaller, cheaper and faster computers, better programming technologies like Assembly language, FORTRAN and COBOL were on the rise and made computer programming more efficient and affordable. Fast forward to the 1970s which gave rise to the more familiar personal computers that we use today with graphical user interfaces. Some of the computers released in that decade include the Apple II and the TRS-80. Newer programming languages like C and BASIC made it easier to program operating systems and applications. Those modern computers and software would then influence modern-day technologies like the Android and iOS operating systems, Windows and Macintosh computers, and programming languages like Java and C#. All of the computing technologies that we take for granted today was built off the back of many people/teams over many years.

### Demonstrate an understanding of the history and principles of software engineering

The term "Software Engineering" was coined in the 1960s by Margaret Hamilton while she was working on navigational systems at NASA for the Apollo mission. Instead of software being seen as a small component of a bigger system, NASA realized how critical software was in the success of the mission. By the end of the decade, software engineering best practices were being discussed at the NATO Software Engineering Conferences. In the 70s and 80s, modern programming languages like C and C++ are created. These new software technologies enable the development of modern operating system like Unix and other Unix-based systems. In the 1990s while working at CERN, Tim-Berners Lee comes up with the idea of a document information system in which documents/resources link to each other over an internet connection. He creates the first web browser known as "WorldWideWeb" (software) and his ideas ultimately help give rise to what we know as the World Wide Web (internet) today.

There are many different principles within Software Engineering space, but the most well known set of principles in modern Software Development are SOLID and DRY.

SOLID standing for:
- Single Responsibility Principle
    - The idea here is when developing software, each class within our software program should focus on a specific task and not deviate from that. For example, we might create a class that is meant to handle client requests to an API. All this class is responsible for is fetching and returning data. Nothing more. We **should not** add another responsibility such as transforming data, storing data or showing the GUI to this class.
- Open-Closed Principle
    - This principle is about keeping our classes **closed to modification** but **open to extension**. The idea here is to create entities (classes, interfaces, etc.) that enabled flexibility and extendability. For example, we might be building UI components and we need a generic "hoverable" component that can represent different kinds of components (text, buttons, containers, etc.). Instead of creating a `Hoverable` class that will likely need modification overtime when we have new requirements, we can create a `Hoverable` *interface* that separate UI component classes can implement in their own way.
- Liskov Substitution Principle
    - This principle has to do with subclasses and inheritance. In any given situation, a subclass should be able to substitute for its parent class without any unexpected output/results. For example, we may have a base `Laptop` class that has subclasses `Macintosh` and `Windows`. We expect that when we call the `toString()` method on a `Laptop` object, it prints the name, model, and specifications of the device. If the `Macintosh` object prints its memory address where we expect to see laptop details, that's a violation of the Liskov Substitution Principle.
- Interface Segregation Principle
    - The idea here is to create multiple interfaces for specific functionality rather than creating a single general-purpose interface.
- Dependency Inversion Principle
    - The Dependency Inversion Principle is about preventing tight coupling by depending on general-purpose and concrete classes. As exemplified in the Open-Closed Principle, our classes should instead depend on flexible interfaces and abstract classes.

and DRY for "Don't Repeat Yourself". If we are following the DRY principle, we are writing code that reduces code redundancy; keeping our code modular and re-usable. An example of this is using constructs like classes, interfaces, and higher-order functions.

### Demonstrate an understanding of the history and principles of data management

Data management refers to the act of collecting, storing, and utilizing data to the best of our ability using industry best practices. Struggling with handling data the previous decades, organizations started practicing data management formally in the 1960s. Back then, data management involved storing data in physical things like punch cards which were stored in data warehouses. As computer technology advanced in areas like storage and software, data management became easier and more efficient. In the 70s, Ted Codd of IBM came up with the Relational Database Model which stores data in tables of related information. He also developed the SQL language. As ideas and technologies in the space improved, Database Management Systems like Oracle and IBM DB2 - which are based off of Codd's ideas - were created and are sold to customers needing Database Management solutions. In the 90s and early 2000s data become more valuable than ever and new solutions like NoSQL databases are developed. Data Science and Management become more important as data is seen as an increasingly valuable asset.

There are many principles when it comes to data collection and management, most of which have to do with data science. First, since we're often dealing with different types of variables (names, locations, numbers, etc.) it helps to organize the data. We often are dealing with two types of variables:
- Numerical
    - These are variables that measure something; they typically have a number and a unit of measurement. For example, "5 miles" or "30 minutes".
- Categorical
    - These are variables that categorize something; they typically represent a number of choices. For example, the number "1" on a "1 - 5 scale" or "Doberman" in a list of dog breeds.

There are other principles when it comes to data collection like insuring data validity and removing bias from data analysis. For example, being aware of confirmation bias is important so that we are not interpreting data in a way that supports our own original views or hypothesis.


### Demonstrate an understanding of the history and principles of networking fundamentals

Just like Data Management, we'll find Computer Networking in its infancy in the 1960s with ARPANET (Advanced Research Project Agency Network) being one of the first wide-area computer networks. ARPANET took from many ideas developed in the 50s and 60s such as TCP/IP (Transmission Control Protocol/Internet Protocol) and packet switching/sending data via "packets." ARPANET influenced future networks like SATNET, BITNET, and ARCNET, and influenced the world-wide network which we know today as the Internet. In the 70s, Ethernet, created by Robert Metcalfe of Xerox, would eventually start to become the dominant computer networking standard due to its flexibility and cost effectiveness. Wi-Fi, ethernet's wireless counterpart, was created in the 1980s and uses many of the standards from [IEEE 802](https://en.wikipedia.org/wiki/IEEE_802). 

Networking today, for the most part, is based on the OSI (Open System Interconnect) Model which describes network operations and communication. The OSI Model gives us a way to categorize and order the different networking protocols used for transferring data to and from devices. The OSI Model is usually represented in "layers":
- Physical Layer (Layer 1)
    - Represents the physical devices within a network like computers, cables, and radio towers which are responsible for transmitting the data. This data may take on different forms as it's passed from one medium to another.
- Data Link Layer (Layer 2)
    - Represents the mechanism that allow us to transfer data to and from physical devices. It include the core protocols and rules that start and stop connections between devices. This is the layer where protocols like Ethernet and DOCSIS-3 function.
- Network Layer (Layer 3)
    - Deals with routing data or "packets" over the physical layer. This is where Internet Protocol (IP) addressing and routing come in. In order for a physical device to send and/or receive data over the internet, it needs a unique address that identifies it.
- Transport Layer (Layer 4)
    - Takes care of the the rules and control flow of data in sessions between devices using standards like Transmission Control Protocol (TCP). 
- Session Layer (Layer 5)
    - Deals with orchestration (open, close, resume, etc.) of communication channels (sessions) between devices.
- Presentation Layer (Layer 6)
    - Defines the mechanisms for encoding and decoding data that is created or needed by the application layer.
- Application Layer (Layer 7)
    - Defines rules regarding end-user applications like web browsers and email clients. This is where Hypertext Transfer Protocol (HTTP) and File Transfer Protocol (FTP) come into the picture.

### Demonstrate an understanding of the history and principles of infrastructure

> Assuming this question is about software infrastructure.

The first programs written for a computer were written by Ada Lovelace for Charles Babbage's Analytical Engine. Early computer programs were written on paper, "punched" cards, and "punched" tape. Software infrastructure evolved as computer hardware improved. As advances were made in the digital computer to be able to store programs in-memory, software became easier and more efficient to write and run. Improvements in software infrastructure also came as a result of programming language/compiler advancement. Instead of writing software in machine-specific binary and/or assembly language, software engineers could write in a consistent english-like general-purpose language (e.g., COBOL, BASIC) on supported devices. As business and user needs became more complex, new and improved processors, compilers, storage, best practices, and architecture needed to be created. This brings us to today's era of cloud computing where a lot of our software is run on a company's servers in a warehouse somewhere far from our physical location. This has allowed companies of all sizes to take advantage of modern computing technology without having to take on the cost of managing their own hardware/software infrastructure.

### Demonstrate an understanding of the history and principles of integrated development environments

Integrated Development Environments (or IDEs for short) aim to combine tools for software development into a single program to make development more efficient. Historically, programs like text editors (e.g., nano, vi), debuggers (e.g., dbx, GDB), and compilers (e.g., make, GCC) where separate. That may still be true today, but good IDEs integrate all of these tools so well to make them seem as a single program. IDEs typically contain a text editor, syntax highlighting, multi-language support, code completion, debugger, complier, version control support, and more. Some popular IDEs today are Visual Studio, Jetbrains IntelliJ, Apache Netbeans, Android Studio, and XCode.