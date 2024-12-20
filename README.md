java cCHC5223 Data Structures and Algorithms 2023-2024-2 
 1 of 6 
Assignment 
Value 100% of Coursework Resit 
Individual work 
Background 
The subway system of a city is a network of underground or elevated trains that provide 
rapid transit for passengers within the urban area. It typically consists of interconnected 
lines or routes, each with designated stops or stations where passengers can board or 
disembark. Subway systems are a vital component of urban transportation infrastructure, 
offering a convenient and reliable mode of travel for commuters, tourists, and residents 
alike. Subway stations are strategically located at key points throughout the city. 
There are several terms used to describe the subway system: 
• Station: is a designated node along a subway line where trains stop to allow 
passengers to board or alight. 
• Terminal Station: is the endpoint of a subway line or route where trains 
begin or end their journeys. 
• Interchange Station: is a crucial component of a subway system. It is a 
station where passengers can transfer between different subway lines or 
routes without exiting the transit system. 
• Route: refers to the path that a subway train follows between two or more 
stations. 
• Line: is a set of interconnected routes that share a common designation and 
usually serve a specific geographic area or corridor within a city. Each line is 
identified by a unique name or number and is represented by a distinct color 
on maps and signage. 
 
 CHC5223 Data Structures and Algorithms 2023-2024-2 
 2 of 6 
General requirements 
This coursework is to write a project to simulate a subway system according to 
one subway map provided as an appendix file named Subway Map of 
Chengdu(2019).png. The map depicts the operation of metro lines in Chengdu as 
of the end of 2019. It provides the information the project needs. 
The following figure is a thumbnail of the map. You’d better view the appendix 
file directly for the high-resolution details. 
 
Note: 
You must create the corresponding graph based on the appendix file exactly. 
• Node 
You only need to consider the termination station and interchange station in the 
map as nodes of the graph. 
• Route 
You only need to consider the colored lines in the map as a route of the graph, 
please ignore the grey lines that mean the planning route not in service at that 
time. 
• Edge 
The distance/cost between two nodes should be labeled as the number of 
sections that exist in real. 
 
 CHC5223 Data Structures and Algorithms 2023-2024-2 
 3 of 6 
Submission Format Requirements 
When you have completed all tasks, you should be able to generate one 
executable project, otherwise you will lose all marks. 
The coursework submitted should be composed of two files： 
• a report as a Microsoft Word document containing a description and explanation 
of the encoding work. 
➢ filename format: Student ID_CHC5223_CW_Resit_Report.docx 
 
• a .zip file containing the project source code files: 
➢ all the project’s source files, including those provided. 
➢ filename format: Student ID_CHC5223_ CW_Resit_Project.zip 
If you do not submit the files according to the requirements, you may lose 10 
marks for the coursework. 
 
 CHC5223 Data Structures and Algorithms 2023-2024-2 
 4 of 6 
Requirements 
Task 1 
Please fill in the spreadsheet of the Excel file adjacency matrix.xlsx provided to 
complete the adjacency matrix according to the map. 
Each node should be named as the abbreviation of the first letters of the station 
name shown on the map. For instance, the station Weijianian should be 
instantiated as wjn. 
Each edge should be labeled as the distance(cost) between two nodes. For 
instance, the edge between Weijianian Station and North Railway Station should 
be labeled as 2. If there is not an edge between two nodes or on itself, 
distance/cost is “Infinite”. 
Tip: There are several examples written for reference in the adjacency matrix. 
代 写CHC5223、Java
代做程序编程语言10 marks 
 
Task 2 
Please create one project in the IDE based on the start code files provided. You 
may modify the files to make the project executable upon completion. 
5 marks 
 
Task 3 
The class Station is a class defined to represent subway stations that are the 
terminal stations or interchange stations. The attribution ‘name’ represents the 
name of the subway station. The attribution ‘line’ is an array list to record the line 
numbers that the station is located at. The attribution ‘previous’ is used to record 
the previous station in which the shortest path. The attribution ‘g_value’ is used to 
record the g_value for the pathfinding algorithm. The attribution ‘previous’ is 
used to record which node is the previous one during finding the shortest path. 
The attribution ‘isTermination’ is used to represent the station as a termination 
station(true) or interchange station(false). 
You must write the corresponding code in the Station.java file based on the 
notations. 
10 marks 
Explain the encoding work in the report rationally and explicitly. 
10 marks 
 
Task 4 
The class subwayMap is used to generate the graph that represents the subway 
map. The nodes of the graph are the termination stations and interchange CHC5223 Data Structures and Algorithms 2023-2024-2 
 5 of 6 
stations of the subway. The edges of the graph are the lines between two 
stations. The attribution ‘stations’ is used to record all stations that exist on the 
subway map. The attribution ‘stationIndex’ represents the index of one station. 
The attribution ‘stationMap’ is used to record the pairing key-value of the station 
and station index. The attribution ‘size’ represents the number of stations. The 
‘adjacencyMatrix’ is a two-dimensional array to record all edges’ distance(cost). 
You must write the corresponding codes in the subwayMap.java file based on the 
notations. 
10 marks 
Explain the encoding work in the report rationally and explicitly. 
10 marks 
 
Task 5 
The class Main is used to generate a graph that can represent the subway of 
Chengdu at the end of 2019 according to the appendix file. 
• In this class, you need to create all stations according to the appendix file. In 
this class, you need to create an object of subwayMap to represent the 
subway system of Chengdu according to the appendix file. 
5 marks 
 
Task 6 
In the Main class, you need to implement the DFT(depth-first traversal) and 
BFT(breadth-first traversal) algorithms to traverse all stations on the map. 
• The implementations of DFT and BFT algorithms can display the process of the 
traversal, including station name, station type, and subway line number information 
in the sequence of the traversal. 
• The station type should be displayed as ‘termination’ or ‘interchange’ according to 
the station’s status. There is an example shown for reference in the following 
screenshot. 
 
• The start station must be the ‘Tianfu Square’ station. 
10 marks CHC5223 Data Structures and Algorithms 2023-2024-2 
 6 of 6 
Explain the encoding work in the report rationally and explicitly. 
 10 marks 
 
Task 7 
In the Main class, you need to implement Dijkstra’s algorithm to find the shortest 
path from ‘East Chengdu Railway Station’ to ‘Taipingyuan’ station. 
• The implementations of Dijkstra’s algorithms can display the information of the 
pathfinding process, including the station name of each station in the closed set and 
open set, the g_value of the station node, or other information that may be 
necessary. There is an example shown for reference in the following screenshot. 
 
• The implementation of Dijkstra’s algorithm can display the shortest path found. 
There is an example shown for reference in the following screenshot. 
 
Tip: You may modify the Station class to make each object of it can be comparable. 
10 marks 
Explain the encoding work in the report rationally and explicitly. 
10 marks 
 
         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
