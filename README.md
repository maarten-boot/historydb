# historydb
a database format for historical events


tables:

eventType:
    id: <uuid>
    name: <utf8-string>
    description: utf8-text

exanple:
    Person:
    Historical:
    Geological: describes very long time events of geological time span
    Astronomical:

tags:
    id: <uuid>
    name: <utf8-string>
    description: utf8-text

example:
    Artist
    Painter
    Poet

    Science
    Ice-Age
    Flood

event:
    id: <uuid>
    name: <utf8-string>
    start: <dateTime>
    end: <dateTime>
    type: fk: <eventTYpe>
    description: utf8-text
    tags: tag...

example
    name: W.A. Mozart
    type: Person
    start
    end
    tags: Musician
