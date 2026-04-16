# Person

![Status: Formed](https://img.shields.io/badge/status-formed-brightgreen)

This folder contains versioned model files for use with the [National Gallery Dynamic Modeller](https://research.nationalgallery.org.uk/lab/modelling/). Models are expressed as tab-separated triples aligned to CIDOC CRM and related extension ontologies.

## Ontologies

See [`ONTOLOGIES.md`](../ONTOLOGIES.md) for full version details, source links, and compatibility notes. Ontologies currently in use:

| Ontology | Version | Prefix |
|----------|---------|--------|
| [CIDOC CRM](https://cidoc-crm.org/html/cidoc_crm_v7.1.3.html) | 7.1.3 | `crm` |
| [CRMdig](https://cidoc-crm.org/extensions/crmdig/html/CRMdig_v4.0.html) | 4.0 | `crmdig` |
| [CRMsci](https://cidoc-crm.org/crmsci/ModelVersion/crmsci-3.0) | 3.0 | `crmsci` |
| [ResearchSpace](https://github.com/researchspace/researchspace) | _see notes_ | `rs` |

## Model versions

<details>
<summary><strong>Person</strong>: latest version <a href="https://research.nationalgallery.org.uk/lab/modelling/?url=https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v1.2.tsv">v1.2</a></summary>

| | Version | Created | Last modified | Open in Modeller |
| :---: | :---: | :---: | :---: | --- |
| :heavy_check_mark: | v1.2 | 2026-03-09 | 2026-04-13 | [Open](https://research.nationalgallery.org.uk/lab/modelling/?url=https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v1.2.tsv) |
|  | v1.1 | 2026-03-07 | 2026-03-09 | [Open](https://research.nationalgallery.org.uk/lab/modelling/?url=https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v1.1.tsv) |
|  | v1.0 | 2026-03-07 | 2026-03-07 | [Open](https://research.nationalgallery.org.uk/lab/modelling/?url=https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v1.0.tsv) |
|  | v0.9 | 2026-03-07 | 2026-03-07 | [Open](https://research.nationalgallery.org.uk/lab/modelling/?url=https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v0.9.tsv) |

</details>

## Field reference

This table lists the fields defined for data entry or display, derived from `//field` and `//field-via` directives in the model. See the [forms folder](../../forms/field-tables.md) for the aggregated cross-model view.

[`models/person`](../models/person/) | [v1.2](https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v1.2.tsv) | [Open in Modeller](https://research.nationalgallery.org.uk/lab/modelling/?url=https://raw.githubusercontent.com/ed-burnett-NG/HPSWG-Models/refs/heads/main/models/person/person_v1.2.tsv)

This model identifies a person with PIDs, labels, and descriptions; records name parts and honorifics, external identifiers and web presence, research disciplines, life dates, affiliations, and optional contact details and residence.

_An individual (historic or modern) acting in research, conservation, authorship, etc._

| Required | Human understandable Label | Alternative Labels | CRM Code | Behaviour | Label Description |
|----------|---------------------------|-------------------|----------|-----------|-------------------|
| ✓ | Persistent Identifier (PID) | External ID | E42 | ![behaviour: External ID](https://img.shields.io/badge/%2F%2F-External%20ID-0e7490) | A globally resolvable identifier for the person (e.g., Wikidata QID, ISNI). |
| Optional | Unique System Label or ID | System Label or ID; Database or System ID/Label | E41 | ![behaviour: System ID](https://img.shields.io/badge/%2F%2F-System%20ID-57606a) | Required within some documentation or database systems, such as ResearchSpace required label. |
| Optional | Given Name | First Name | E41 | ![behaviour: Free Text](https://img.shields.io/badge/%2F%2F-Free%20Text-0969da) | The person's given/first name as an appellation. |
| Optional | Family Name | Surname | E41 | ![behaviour: Free Text](https://img.shields.io/badge/%2F%2F-Free%20Text-0969da) | The person's family/last name as an appellation. |
| Optional | Honorific / Title | -- | E41 | ![behaviour: Controlled List](https://img.shields.io/badge/%2F%2F-Controlled%20List-1a7f37) | Honorifics or titles (e.g., Dr, Prof, Sir). |
| Optional | Description Text | Person Description | E73 | ![behaviour: Free Text](https://img.shields.io/badge/%2F%2F-Free%20Text-0969da) | Free-text biographical or role description. |
| Optional | Place (Residence) | Residence of Person | E53 | ![behaviour: Select Entity](https://img.shields.io/badge/%2F%2F-Select%20Entity-8250df) | A place where the person lives/lived. |
| Optional | Organisation (Affiliation) | Affiliated Organisation | E74 | ![behaviour: Select Entity](https://img.shields.io/badge/%2F%2F-Select%20Entity-8250df) | An organisation or group the person is/was affiliated with or a member of. |
| Optional | Birth Date | Date of Birth; Year Born | E52 | ![behaviour: Free Text](https://img.shields.io/badge/%2F%2F-Free%20Text-0969da) | Time-span for birth. |
| Optional | Death Date | Date of Death; Year Died | E52 | ![behaviour: Free Text](https://img.shields.io/badge/%2F%2F-Free%20Text-0969da) | Time-span for death. |

## Contributing

If you would like to contribute to this model, please refer to the [repository contributing guidelines](../../CONTRIBUTING.md) and the [ontology reference](../../ONTOLOGIES.md). The TSV triple format is documented in the [Dynamic Modeller](https://research.nationalgallery.org.uk/lab/modelling/) interface.
