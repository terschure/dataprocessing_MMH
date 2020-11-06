# OBITools demultiplexing

The raw data for this project is divided over 3 pools, representing the PCR replicates of the faecal samples. 
The first steps in the dataprocessing are therefore in parallel for these 3 PCR pools, each PCR pool also needing a seperate sample description file for the demultiplexing using OBITools *ngsfilter*:
 - pool1_description_a.txt
 - pool2_description_b.txt
 - pool3_description_c.txt
 
The sample names used in these sample descriptions contain the following information:
[sample_number]_[group]_[label]_[herbivore_name]_[percentage_identity]_[#primerpairs]_[replicate]

[group] can be 'd' for domestic or 'w' for wild
[label] is the herbivore identity based on visual identification at sample collection
[herbivore_name] is the herbivore identity based on herbivore DNA analysis
[percentage_identity] is the percentage identity from herbivore DNA analysis
[#primerpairs] is the number of primer pairs that gave a positive ID based on herbivore DNA analysis
[replicate] can be 'a', 'b', 'c' and represent the different PCR replicates used for the plant DNA amplification 

The [label] and [herbivore_name] abbreviations stand for:

0 - blank
A - Asian palm civet
BD - Barking deer
BU - Buffalo
C - Cattle
E - Elephant
G - Domestic goat
M - Bonnet macaque
P - Indian porcupine
R - Indian hare
SA - Sambar deer
SB - Sloth bear
W - Wild boar
