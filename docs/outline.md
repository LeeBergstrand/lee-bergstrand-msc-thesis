Thesis High Level Outline
=========================

Introduction
------------
- The problem
- Status quo
- Importance of visualization
- Current things that address the problem
- Our solution
- Selection of a properties database
- Overview of Genome Properties

Chapter One (Pygenprop)
-----------------------
- Introduction and design intentions
- Development of a parser for the genome properties database
   - An introduction to the genome properties file format
   - Description of the parser
   - Parser performance metrics
- Development of an object oriented class framework for the representation of the Genome Properties database  
   - The genome property class
   - The literature reference class
   - The database reference class
   - The Step class
   - The Functional Element class
   - The Evidence class
   - The Genome Property Tree class
- Process of assignment of Genome Properties
   - The Assignment Cache class
   - Assignment of property steps
   - Assignment of properties
- Development of a representation for comparing genome property assignments across multiple organisms
   - The assignment results class
   - The choice of pandas
   - Example workflows
   - Compatibility with python data science stack
   - Compatibility with python machine learning stack
- Development of a file storage format and database interface for genome property assignment storage
   - Selection of a data storage format
   - Advantages of an ORM and database connectivity
   - The schema of Micromeda file format
- Extension of assignment caches and assignment results class to include supporting match information
  - The purpose of adding match information
  - Considerations for adding match information
  - The extended assignment cache class
  - The extended assignment result class
- Development of a in memory transfer format for genome property assignments and supporting match information
  - The purpose of an in-memory serialization format
  - The selection of msgpack
- Automated testing and deployment
- Future improvements
   - Normalize the step matches data frame into separate match and sequence data frames
   - Speed up writing and reading to the SQLite file
   - Use the to message pack instead of SQLite
- Summary 

Chapter Two (Annotation Pipeline)
---------------------------------
- Why we need a pipeline
- Development of an easily installable version of InterProScan
- The genome pipeline
- The metagenome pipeline
  - Considerations for metageneome analysis
  - Performance comparison
- Future improvements

Chapter Four (Micromeda Server)
-------------------------------
- The intent 
- The architecture

Chapter Three (Micromeda Client)
--------------------------------
- Introduction and design intentions
- Visualization philosophy
- Overview of design
- Comparison to competing designs
- Future improvements

Conclusions
-----------
