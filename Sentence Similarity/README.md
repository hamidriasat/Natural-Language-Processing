
### AI Test Task
Auto suggest best related observations. 

###### Input

User will type an observation e.g: 

Face and eye protection equipment shall be kept clean …

###### Output

Then User shall be given 3-5 suggested observations. E.g:

- Face and eye protection equipment shall be kept clean and in good repair. The use of this type equipment with structural or optical defects shall be prohibited.
- Containers shall be provided for the collection and separation of waste, trash, oily and used rags, and other refuse. Containers used for garbage and other oily, flammable, or hazardous wastes, such as caustics, acids, harmful dusts, etc. shall be equipped with covers. Garbage and other waste shall be disposed of at frequent and regular intervals.
- "Application." Protective equipment, including personal protective equipment for eyes, face, head, and extremities, protective clothing, respiratory devices, and protective shields and barriers, shall be provided, used, and maintained in a sanitary and reliable condition wherever it is necessary by reason of hazards of processes or environment, chemical hazards, radiological hazards, or mechanical irritants encountered in a manner capable of causing injury or impairment in the function of any part of the body through absorption, inhalation or physical contact.
- "Application." Protective equipment, including personal protective equipment for eyes, face, head, and extremities, protective clothing, respiratory devices, and protective shields and barriers, shall be provided, used, and maintained in a sanitary and reliable condition wherever it is necessary by reason of hazards of processes or environment, chemical hazards, radiological hazards, or mechanical irritants encountered in a manner capable of causing injury or impairment in the function of any part of the body through absorption, inhalation or physical contact.
- Employees shall be provided with eye and face protection equipment when machines or operations present potential eye or face injury from physical, chemical, or radiation agents.

###### Required Data
SORs.xlsx is attached to be used as Data.

#### Technique 
Solved using pretrained [bert sentence similarity model "bert-base-nli-stsb-mean-tokens"]( https://github.com/UKPLab/sentence-transformers). 

Using pretrained bert first find sentences simialrty to input sentence.  Then using Cosine similarity pick those sentences whose sentence similarity is greater then some threshold.
