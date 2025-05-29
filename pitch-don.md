---
marp: true
theme: don
transition: wipe
headingDivider: 2
---
# developer.overheid.nl
<!-- _class: title -->

## Kernteam

- Product Owner: Dimitri van Hees
- Developer Advocate: Tom Ootes
- Front-end: Jaap-Hein Wester
- Backend: Matthijs Hovestad

## Implementatieondersteuning

- Joost Farla (architect)
- Martin van der Plas (architect)
- Frank Terpstra (expert standaarden)

## Developer portal

- Kennisbank
- Communities
- Blog
- Tools
- Forum
- API register
- Open Source Software (OSS) register

## Practice what you preach

- Front-end op basis van NL Design System
- Open Source
- API first

## Nieuwe ADR validator

- Compatible met nieuwe versie API Design Rules
- Valideert tegen OAS
- Accepteert afwijkende OAS locatie
- Betere resultaten in API dashboard

## Integratie communities

- Kennisplatform API’s
- Digilab
- OSPO-NL

## Known issues

- Homepage
- Informatiestructuur
- Toegankelijkheid
- Slack en Github

## Focus op REST

- WMS/WFS -> OGC API = REST
- ODATA (4) = "REST"
- GraphQL (1)
- CKAN (1)
- Atom (1)
- Socrata (1)

## OAS first (en hopelijk zsm 3.1)

- Contact info (ADR 2.1)
- Environments (nog niet in ADR)
- Security (mTLS vanaf 3.1)
- Example(s) tbv mocking services en SDK’s
- JSON schemas (vanaf 3.1)

## Nieuwe features

- Nieuwe aanleverprocedure ism Logius
- API lifecycle informatie; actuele versie, deprecation, uptime
- Verbeterde developer experience; functionele documentatie, tooling, mock data, SDK’s, Bruno collections, etc.
- Toegankelijke front-end obv NL Design System
- Filteren/zoeken
- Verbeterde contactinformatie
- Embedded Discourse comments

## Schema

```json
{
  "$id": "https://example.com/person.schema.json",
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "title": "Person",
  "type": "object",
  "properties": {
    "firstName": {
      "type": "string",
      "description": "The person's first name."
    },
    "lastName": {
      "type": "string",
      "description": "The person's last name."
    },
    "age": {
      "description": "Age in years which must be equal to or greater than zero.",
      "type": "integer",
      "minimum": 0
    },
    "age": {
      "description": "Age in years which must be equal to or greater than zero.",
      "type": "integer",
      "minimum": 0
    }
  }
}
```
