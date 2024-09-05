# Mike Ross - US Lawyer

@prefix : <http://example.org/law#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix sh: <http://www.w3.org/ns/shacl#> .
@prefix shex: <http://www.w3.org/ns/shex#> .

# Define Classes
:Person rdf:type rdfs:Class ;
    rdfs:label "Person" ;
    rdfs:comment "A human being." .

:Lawyer rdf:type owl:Class ;
    rdfs:subClassOf :Person ;
    rdfs:label "Lawyer" ;
    rdfs:comment "A person who practices or studies law; an attorney or a counselor." .

:LegalCase rdf:type rdfs:Class ;
    rdfs:label "Legal Case" ;
    rdfs:comment "A dispute between two parties that is resolved in a court of law." .

:USLawResource rdf:type rdfs:Class ;
    rdfs:label "US Law Resource" ;
    rdfs:comment "A resource related to the legal system of the United States." .

:SourceOfUSLaw rdf:type rdfs:Class ;
    rdfs:label "Source of US Law" ;
    rdfs:comment "An authoritative legal source in the US legal system." .

# Define Properties
:name rdf:type rdf:Property ;
    rdfs:domain :Person ;
    rdfs:range xsd:string ;
    rdfs:label "Name" ;
    rdfs:comment "The name of a person." .

:occupation rdf:type rdf:Property ;
    rdfs:domain :Person ;
    rdfs:range :Lawyer ;
    rdfs:label "Occupation" ;
    rdfs:comment "The occupation of a person." .

:handlesCase rdf:type rdf:Property ;
    rdfs:domain :Lawyer ;
    rdfs:range :LegalCase ;
    rdfs:label "Handles Case" ;
    rdfs:comment "The legal cases that a lawyer handles." .

:referencesResource rdf:type rdf:Property ;
    rdfs:domain :Lawyer ;
    rdfs:range :USLawResource ;
    rdfs:label "References Resource" ;
    rdfs:comment "The US law resources that a lawyer references." .

:isSourceFor rdf:type rdf:Property ;
    rdfs:domain :USLawResource ;
    rdfs:range :SourceOfUSLaw ;
    rdfs:label "Is Source For" ;
    rdfs:comment "The source of a US law resource." .

# Define Individuals
:MikeRoss rdf:type :Lawyer ;
    :name "Mike Ross" ;
    :occupation :Lawyer ;
    :handlesCase :Case1 ;
    :referencesResource :Resource1, :Resource2 .

:Case1 rdf:type :LegalCase ;
    rdfs:label "Case 1" ;
    rdfs:comment "A legal case handled by Mike Ross." .

:Resource1 rdf:type :USLawResource ;
    rdfs:label "Resource 1" ;
    rdfs:comment "A US law resource referenced by Mike Ross." ;
    :isSourceFor :Source1 .

:Resource2 rdf:type :USLawResource ;
    rdfs:label "Resource 2" ;
    rdfs:comment "Another US law resource referenced by Mike Ross." ;
    :isSourceFor :Source2 .

:Source1 rdf:type :SourceOfUSLaw ;
    rdfs:label "Source 1" ;
    rdfs:comment "An authoritative source of US law." .

:Source2 rdf:type :SourceOfUSLaw ;
    rdfs:label "Source 2" ;
    rdfs:comment "Another authoritative source of US law." .

# Define SHACL Shapes
:LawyerShape a sh:NodeShape ;
    sh:targetClass :Lawyer ;
    sh:property [
        sh:path :name ;
        sh:datatype xsd:string ;
        sh:description "The lawyer's name should be a string." ;
        sh:minCount 1 ;
    ] ;
    sh:property [
        sh:path :handlesCase ;
        sh:nodeKind sh:IRI ;
        sh:description "A lawyer should handle at least one case." ;
        sh:minCount 1 ;
    ] ;
    sh:property [
        sh:path :referencesResource ;
        sh:nodeKind sh:IRI ;
        sh:description "A lawyer should reference at least one US law resource." ;
        sh:minCount 1 ;
    ] .

# Define ShEx Schema
:LawyerShape {
    :name xsd:string ;
    :handlesCase IRI ;
    :referencesResource IRI ;
}
