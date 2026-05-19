# Codelijst CSOR — Kwalificeerbaar aspect

Deze repository bevat de SKOS-codelijst **Kwalificeerbaar aspect** binnen het CSOR-datamodel (Chemische Stoffen en Omgevingsparameters-Register) van de Vlaamse overheid.

## Beschrijving

Een kwalificeerbaar aspect drukt uit dat de waarde die aan een observatie kan worden toegekend, beperkt is tot classificaties opgenomen in een elders gepubliceerde lijst.

- Concept scheme URI: `https://data.omgeving.vlaanderen.be/id/conceptscheme/csor/kwalificeerbaaraspect`
- Namespace: `https://data.omgeving.vlaanderen.be/ns/csor#`
- Named graph (Virtuoso): `https://data.omgeving.vlaanderen.be/id/graph/codelijst-csor-kwalificeerbaar-aspect`

## Bestandsstructuur

```
src/main/resources/be/vlaanderen/omgeving/data/id/conceptscheme/csor/kwalificeerbareaspect/
├── kwalificeerbareaspecten.ttl           # Turtle-serialisatie (hoofdbestand)
├── kwalificeerbareaspecten.nt            # N-Triples-serialisatie
├── kwalificeerbareaspecten.rj            # RDF/JSON-serialisatie
└── kwalificeerbareaspecten_report.ttl    # SHACL-validatierapport
```

## Gebruikte standaarden

| Prefix | Namespace | Doel |
|--------|-----------|------|
| `skos` | `http://www.w3.org/2004/02/skos/core#` | Concept scheme structuur |
| `csor` | `https://data.omgeving.vlaanderen.be/ns/csor#` | CSOR-specifieke eigenschappen |
| `sh` | `http://www.w3.org/ns/shacl#` | SHACL-validatie |
| `iadopt` | `https://w3id.org/iadopt/ont/` | I-ADOPT observatieraamwerk |

## Validatie

Het bestand `kwalificeerbareaspecten_report.ttl` bevat het SHACL-validatierapport. Elk kwalificeerbaar aspect dient exact één `csor:classificatielijst` te hebben.

## Licentie

[GNU General Public License v3](LICENSE)
