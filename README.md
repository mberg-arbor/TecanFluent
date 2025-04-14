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



[Tecan Support Blog 3rd Party](https://labautomation.io/c/tecan/8) <br />
[Tecan Fluent Worklisting and Keeping Tips on](https://labautomation.io/t/tecan-fluent-worklisting-and-keeping-tips-on/2112)
-For example the Tecan generated format might look like this below. I’ve tried removing the W; after each A and D set, it didn’t like that. <br />
A;Water[001];;;A1;;6.51;;;; <br />
D;NormalizationPlate[001];;;A1;;6.51;;;; <br />
W; <br />
A;Water[001];;;A1;;7.88;;;; <br />
D;NormalizationPlate[001];;;C1;;7.88;;;; <br />
W; <br />
A;Water[001];;;A1;;7.87;;;; <br />
D;NormalizationPlate[002];;;E1;;7.87;;;; <br />
W; <br />
A;Water[001];;;A1;;5.76;;;; <br />
D;NormalizationPlate[002];;;F1;;5.76;;;; <br />
W; <br />

[Execute worklist with all 8 tips](https://labautomation.io/t/execute-worklist-with-all-8-tips/3989/1) <br />
In this blog they are working to set up setting up transfering different volumes into wells of a 96 plate. They are asking for help troubleshooting an issue in the Freedom EVO softwear so while this isnt 
softwear for us, it still contains a another example of the instruction files for the pipetting steps

[Tecan Worklist (.gwl) - liquid handling with specific LiHa tips](https://labautomation.io/t/tecan-worklist-gwl-liquid-handling-with-specific-liha-tips/3843) <br />
This is another person using FreedomEVO so its slightly different but the worklist the provide is again another example of the gwl file set up 

[Tecan .gwl scripting - Mix](https://labautomation.io/t/tecan-gwl-scripting-mix/4533) <br />
Final exmple of worklist set up I swear lol




