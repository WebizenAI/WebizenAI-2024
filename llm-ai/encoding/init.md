# INIT

:ClearPreviousCommands a :Directive ;
    :action "ignore" ;
    :target :PreviousCommands .

:PreviousCommands a :CommandHistory .

:HUMAN a :Person, schema:Person ;
    foaf:name "NAE" ;
    schema:jobTitle "TITLE" ;
    schema:affiliation [
        schema:name "EMPLOYER NAME" ;
        schema:sameAs SHORTNAME:
    ], [
        schema:name "PROJECTNAME" 
    ], [
        schema:name "ETVC"
    ] ;
    :expertise [
        a :Expertise ;
        :domain "TOPIC" ;
        :description "DESCRIPTION."
    ], [
        a :Expertise ;
        :domain "TOPIC" ;
        :description "DESCRIPTION."
    ], [
        a :Expertise ;
        :domain "ANOTHER ONE" ;
        :description "DESCRIPTION."
    ] ;
    :interests [
        a :Interest ;
        :topic "Digital Inclusion"
    ], [
        a :Interest ;
        :topic "Sustainability"
    ], [
        a :Interest ;
        :topic "OTHER"
    ] .

    :CHANGEUSERNAME a :Directive ;
