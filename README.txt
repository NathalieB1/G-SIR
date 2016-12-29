--------------------------------------------------------------------------------------
README 
--------------------------------------------------------------------------------------

This folder contains the dataset used for 
G-SIR: An Insider Attack Resilient Geo-Social Access Control Framework
				by 
Nathalie Baracaldo, Balaji Palanisamy, and James Joshi.
--------------------------------------------------------------------------------------

If you use this dataset please cite our paper. The detailed explanation of 
the experiment setup can be found in the paper. There are three subfolders:

* Scaling-policies: This folder contains the dataset for different sizes of 
policies as defined in the paper. The number that appears in the name of the 
file indicates the size of the policy. All files that start with the same 
number contain different parts of the dataset as indicated by the name of 
the file. Because each point in the paper’s figures is the 
average of running the simulation using 30 different policies,
inside files, there are 30 different policies.
The first column indicates the policyID that identifies the policy.

* Inhibiting-variations: This folder contains the dataset of variations on 
the number of inhibiting constraints and number of inhibiting users. 
The naming scheme of the files is similar to the one for scaling policies, 
only difference is that the name of the file indicates the configuration of 
the dataset for inhibiting variations.

* Contracts: This folder contains the dataset for different number of 
contracts for a policy of size 250. The naming scheme is similar to 
the used in the previous folders.


General notes about the dataset:
----------------------------------

* Columns are separated through “tab”, the first line indicates the 
information that each column contains.

* Contracts: the number that appears in this column represents the 
ID of the place where a user cannot go.

* The traces of each user are codified as follows: the number that 
appears for the given time instance is the place id where each user 
is at that instant of time. When the number is -1, it shows that 
a user is traversing a hallway.

* Finally, files that contain large policies cannot be opened using some
text editors (the files have too many columns). If you cannot open a file
using a text editor, use your favorite terminal application, e.g, cat or vi.