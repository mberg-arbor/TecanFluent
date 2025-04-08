# TecanFluent
Resources and items for the Tecan Fluent

# Reading Materials 
[FluentControl™ software - Manual](https://www.tecan.com/knowledge-portal/fluentcontrol-software-manual)

# .gwl Files 
A GWL (GeneWorks List) file is a plain test file. Each line is a single command, the FluentControl software reads the file line by line 

`[Command] ; [Source Labware] ; [Source Position] ; [Volume in µL] ; [Destination Labware] ; [Destination Position] ; [Additional Parameters...]`

|Command|	Meaning|	Example|
|-----|----------|------------|
|A|	Aspirate	|`A;SourcePlate;A1;100`|
|D|	Dispense	|`D;DestinationPlate;B1;100`|
|W|	Wash	|`W (just wash tips)`|
|C|	Comment	|`C;This is a comment`|

