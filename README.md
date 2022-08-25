# Forest Observatory Ontology 

The Forest Observatory Ontology (FOO) ( is an ontology for describing wildlife data generated by sensors. FOO's scope evolves around the Internet of Things (IoT) and wildlife habitats. To illustrate our datasets of interest, we modelled the concept to represent "sensors observing animals and land". These sensors generate observations. For example, the animal GPS collar tracks an elephant and records its geo-location observations for different and equally spaced time intervals and temperature every specified time interval. We adopted classes and properties from SOSA and BBC wildlife ontologies to model the domain coverage.


# FOO specification draft
https://github.com/Naeima/Forest-Observatory-Ontology-/releases/download/v1.0.0/index-en.html


# OOPS! (OntOlogy Pitfall Scanner!) results
https://github.com/Naeima/Forest-Observatory-Ontology-/releases/download/v1.0.0/oopsEval.html



![image](https://user-images.githubusercontent.com/57564713/185769396-6a963789-43da-4993-9273-cf2c37256595.png)



# FOO Development

We developed FOO following the Linked Open Terms (LOT) methodology using a complied list of comptency questions (functional requirements)- implemented in protege software.  LOT  was originated from Neon methodology, it encourages borrowing and reusing classes from fully developed and widely shared ontologies. Therefore, we searched the existing literature for suitable ontologies. Then, we decided to borrow classes and relationships from SOSA and the BBC Wildlife Ontology, as they contained sufficient components to model our proposed entities (i.e., instances or individuals). Moreover, LOT recommends sharing ontologies according to the Linked Data principles to enable re-using the ontologies by the research community and software applications. 

![things](https://user-images.githubusercontent.com/57564713/185769351-04be89c3-13fd-47aa-9b17-6298d426d4ae.png)

# Repository
This repository has a copy of the following:

•	A spreadsheet contains the ontology functional requirements (i.e., comptency questions) 

•	Ontology in RDF/XML and TURTLE formats.

•	Ontology documentation using WIDOCO tool





# SPARQL Query example 
What objects do contain the word sensor? 

    PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>.

    PREFIX owl: <http://www.w3.org/2002/07/owl#>.

    PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>.

    PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>.


    SELECT ?subject ?predicate ?object

    WHERE { ?subject ?predicate  ?object.
    
    FILTER REGEX(?object, ("Sensor"))}
    

![sensor](https://user-images.githubusercontent.com/57564713/185769348-497951cf-6b9d-465b-98f8-8a67b99121df.png)

# References

[1] 2022.  https://www.bbc.co.uk/ontologies/wildlife

[2] Daniel Garijo. 2017. WIDOCO: a wizard for documenting ontologies. In International Semantic Web Conference. Springer,
94–102. https://dgarijo.github.io/Widoco/

[3] 2022. OOPS! - OntOlogy Pitfall Scanner! https://oops.linkeddata.es/

[4] 2022. Protégé. https://protege.stanford.edu/

[5] 2022. Semantic Sensor Network Ontology.https://www.w3.org/TR/vocab-ssn/

[6] María Poveda-Villalón, Alba Fernández-Izquierdo, Mariano Fernández-López, and Raúl García Castro. 2022. LOT:An industrial oriented ontology engineering framework. Engineering Applications of Artificial Intelligence 111 (2022), 104755.https://www.sciencedirect.com/science/article/pii/S0952197622000525

[7] Asunción Gómez-Pérez and Mari Carmen Suárez-Figueroa. 2009. NeOn methodology for building ontology networks:a scenario-based methodology (2009), https://oa.upm.es/5475/1/INVE_MEM_2009_64399.pdf

[8] Milena Salgado Lynn and Amaziasizamoria Jumail. 2021. The Danau Girang Field Centre: Field Station Profile.ECOTROPICA 23, 1/2 (2021), 202103–202103. https://www.ecotropica.eu/index.php/ecotropica/article/view/86/26




