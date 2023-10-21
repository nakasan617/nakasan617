<p align='center'>
<a href="https://twitter.com/yutanak6"><img height="30" src="https://github.com/nakasan617/nakasan617/blob/master/blob/twitter.png?raw=true"></a>&nbsp;&nbsp;
<a href="https://www.linkedin.com/in/yuta-nakamura-93b9b778/"><img height="30" src="https://github.com/nakasan617/nakasan617/blob/master/blob/linkedin.svg?raw=true"></a>&nbsp;&nbsp;
<a href="https://www.chess.com/member/nakasan6"><img height="30" src="https://github.com/nakasan617/nakasan617/blob/master/blob/chess.png?raw=true"></a>&nbsp;&nbsp;

</p>

# PROFILE #

Hello this is Yuta Nakamura. I am a Ph.D. candidate at DePaul University (almost in the 3rd year).
I have an enormous curiosity out there and I wish to create some business that would change the game in an industry.

# RESEARCH #

I am currently in computer systems, which does things related to compilers, operating systems, database, etc... I am currently working on research of program analysis. To be more specific, I am trying to create this software to detect the point of divergence/reconvergence of two executions. We are currently assuming those differences occur because of provenances of the 2 executions. 

I love research in a sense that I get to control what I do at my own time schedule, though sometimes it gets packed before the deadlines. 

## PUBLISHED WORK ##

The following is the published work I have so far. 

### Efficient Differencing of System-level Provenance Graphs (2023) ###
Abstract:  
Data provenance, when audited at the operating system level, generates a large volume of low-level events. Current provenance systems infer causal flow from these event traces, but do not infer application structure, such as loops and branches. The absence of these inferred structures decreases accuracy when comparing two event traces, leading to low-quality answers from a provenance system. In this paper, we infer nested natural and unnatural loop structures over a collection of provenance event traces. We describe an `unrolling method' that uses the inferred nested loop structure to systematically mark loop iterations. Our loop-based unrolling improves the accuracy of trace comparison by 20-70\% over trace comparisons that do not rely on inferred structures.

### Provenance-based Workflow Diagnostics Using Program Specification (2022) ###
Abstract:  
Workflow management systems (WMS) help automate and coordinate scientific modules and monitor their execution. WMSes are also used to repeat a workflow application with different inputs to test sensitivity and reproducibility of runs. However, when differences arise in outputs across runs, current WMSes do not audit sufficient provenance metadata to determine where the execution first differed. This increases diagnostic time and leads to poor quality diagnostic results. In this paper, we use program specification to precisely determine locations where workflow execution differs. We use existing provenance audited to isolate modules where execution differs. We show that using program specification comes at some increased storage overhead due to mapping of provenance data flows onto program specification, but leads to better quality diagnostics in terms of the number of differences found and their location relative to comparing provenance metadata audited within current WMSes.
<!--
To increase the repeatability of the workflow system, we have created a tool called ProvScope. Whenever some workflow executions show unexpected outputs, ProvScope compares with same workflow with expected outputs (from a different input) to narrow down the bugs of the workflows. ProvScope uses program specifications to precisely find the points of divergence of the executions, and to deal with the path explosion problem to identify the path in the program specifications from traces, function call traces are used in a hierarchical manner to reduce the search space.
-->

[Link to the paper](https://dice.cs.depaul.edu/pdfs/pubs/C32.pdf)

Published in HiPC 2022

### Content Defined Merkle Tree (2020) ###
Abstract:  
Containerization simplifies the sharing and deployment of applications when environments change in the software delivery chain. To deploy an application, container delivery methods push and pull container images. These methods operate on file and layer (set of files) granularity, and introduce redundant data within a container. Several container operations such as upgrading, installing, and maintaining become inefficient, because of copying and provisioning of redundant data. In this paper, we reestablish recent results that block-level deduplication reduces the size of individual containers, by verifying the result using content-defined chunking. Block-level deduplication, however, does not improve the efficiency of push/pull operations which must determine the specific blocks to transfer. We introduce a content-defined Merkle Tree (\CDMT{}) over deduplicated storage in a container. \CDMT{} indexes deduplicated blocks and determines changes to blocks in logarithmic time on the client. \CDMT{} efficiently pushes and pulls container images from a registry, especially as containers are upgraded and (re-)provisioned on a client. We also describe how a registry can efficiently maintain the \CDMT{} index as new image versions are pushed. We show the scalability of \CDMT{} over Merkle Trees in terms of disk and network I/O savings using 15 container images and 233 image versions from Docker Hub. 

<!--
As I was to implement Merkle tree in [Sciunit](https://sciunit.run/), I realized that Merkle tree cannot be used for blocks that are created with Content-Defined Chunking method. Therefore we came up with the idea of CDMT, which does the Content-Defined Chunking in the internal nodes. This data structure is now robust against the chunk-shift, which occurs using the Merkle trees on top of content-defined chunks. 
-->
[Link to CDMT](https://arxiv.org/abs/2104.02158#:~:text=Containerization%20simplifies%20the%20sharing%20and,push%20and%20pull%20container%20images.)

Published in HiPC 2020

### Efficient Provenance Alignment in Reproduced Executions (2020) ###
Abstract:  
Reproducing experiments entails repeating experiments with changes. Changes, such  as  a change  in  input  arguments, a change in the invoking environment, or a change due  to  non-determinism in the runtime may alter results. If results alter significantly, perusing them is not sufficient---users must analyze the impact of a change and determine if the experiment computed the same steps. Making fine-grained, stepwise comparisons can be both challenging and time-consuming. In this paper, we compare a reproduced execution with recorded system provenance of the original execution, and determine \textit{provenance alignment}. The alignment is based on comparing the specific location in the program, the control flow of the execution, and data inputs. Experiments show that the alignment method has a low overhead to compute a match and realigns with a small look-ahead buffer. 
<!--
[SPADE](https://github.com/ashish-gehani/SPADE) and Sciunit use system calls to trace the provenance of the executions. Therefore this is our first attempt to look at the system call trace to make sure the two executions are aligned. 
-->

[Link to Provenance Alignment](https://www.usenix.org/conference/tapp2020/presentation/nakamura)

Published in TaPP 2020

# HOBBIES #

I love studying and playing chess and other strategic board games, so if you are interested, befriend me and play against me! 
My rating is around 1500 in rapid (10 min) for chess.

[Link to chess.com](https://www.chess.com/member/nakasan6)

