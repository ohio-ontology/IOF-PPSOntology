# IOF-PPS Ontology

Reference ontologies attempt to represent deep knowledge of basic science in aprincipled  way  that  allows them  to be re-used  in  multiple  ways.   The  largeamount of design and manufacturing data generated, stored and exchanged between systems require a proper knowledge representation in formats that makessharing easy.  semantic analysis of the data and development of ontologies forproduct design and manufacturing planning tasks will enable smart manufactur-ing applications (e.g.  cloud manufacturing, AI-based manufacturing, IndustrialIOT, Industry 4.0).

Semantic Data Integration offers a solution that goes beyond the standardenterprise  application  integration  solutions.   It  employs  a  data-centric  archi-tecture built upon a standardized model for data publishing and interchange,namely the Resource Description Framework (RDF).

This is a report on efforts to develop a reference ontology for Process and Production Planning (PPS) and current progress of the corresponding working group within Industrial Ontology Foundry (IOF). The development process is described together with the current draft of the PPS ontology.

Currently, manufacturing engineering processes see the involvement of various managers, engineers, and operators interacting with several software tools, namely Product Life-cycle Management (PLM), Enterprise Resource Planning (ERP), and Manufacturing Execution Systems (MES) with data flowing in both directions.
The development of the PPS ontologies stems from the definition of key use cases and competency questions that will be used for the validation as well. The proposed PPS ontologies will include relevant terms and will be linked to the IOF top level ontology. 

![image](https://user-images.githubusercontent.com/81836259/141977812-ba91e49a-7fb6-4c6d-a257-525ac1ab2e83.png )

<img src="https://user-images.githubusercontent.com/81836259/141977812-ba91e49a-7fb6-4c6d-a257-525ac1ab2e83.png" width="600">

**Figure 1.** Manufacturing enterprise process data flow



**Use Cases**
1. The process planning use case starts with a part design provided as a drawing or a CAD model (which has nominal geometry and tolerance specification) and the goal is to develop one or more process plans that will completely produce a part with given design, considering available production technologies, machines, tools and other resources. Those plans also need to include a sequence of processing steps that will guarantee achievement of prescribed tolerances. Currently in industry various levels of database search are performed (mostly for tools) in CAM tools in order to generate plans with using planners’ experience for capabilities and sequencing, while research prototypes apply rule-based reasoning combined with a search within limited data sources.

2. The production system design use case takes place after process planning has been completed and consists in the definition of production system configurations that are able to reach the production goals while specifying the required production resources, process/resource assignments, layout design, etc. Candidate system configurations may be assessed thanks to performance evaluation methods and tools while iterating the system design loop. Currently, system design employs heterogeneous software tools that are spread among several departments. For example, dynamic performance evaluation (e.g. via discrete event simulation) relies on product and resource data, but simulation software tools do not provide integration paths with PLM/ERP systems.

3. The scheduling optimization use case is a further step towards the operational control of production processes. In addition to process and resource data, scheduling also needs data from customers, i.e. orders and their due dates, suppliers and supplied components/materials lead times, etc. Currently optimization models are executed on separate optimization software, and it is really challenging to integrate their output into ERP and MES systems.


**Process and Production Planning OWL Ontology**
Process and Production Planning ontology has been built by extending the terms definitions based on the upper level ontology (BFO), a few midlevel ontologies (IAO, CCO) , and an IOF reference ontology from industrial applications (IOF core).

Therefore, the draft PPS ontology (Figure 2) includes only terms that extend classes and terms from upper level ontologies. The figure shows relevant classes from BFO (on the top, in orange), a few necessary terms from the CCO ontology (on the left, in yellow), several IOF classes (underneath BFO classes, in light orange). The current development of classes for PPP ontologies shows terms divided into two groups, i.e. design related terms (prefixed with DSGN), and process planning terms (prefixed with MFG). The figure shows only relationships among defined classes. 

![image](https://user-images.githubusercontent.com/81836259/141982535-5ed76256-cbc4-412b-9444-743f56d4673b.png)

<img src="https://user-images.githubusercontent.com/81836259/141982535-5ed76256-cbc4-412b-9444-743f56d4673b.png" width="800">


**Figure 2**. Inheritance hierarchy of PPS ontology terms




