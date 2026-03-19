# Forms and Data Input Resources

This folder contains resources to support the design of forms and data input interfaces derived from the HPSWG semantic models. The materials here are intended for data managers, system implementers, and anyone planning how metadata will be captured in practice.

The semantic models in this repository define how heritage science data is structured and connected using CIDOC CRM. The resources in this folder translate that structure into a more accessible format, identifying which fields are relevant for data entry, their human-readable labels, alternative names, and whether they are required or optional.

## Contents

<!-- AUTO:forms_listing -->
<!-- END:forms_listing -->

## Relationship to the models

The field tables in this folder are generated automatically from `//field` and `//field-via` directives embedded in the TSV model files. If a model does not yet contain these directives it will not appear here. The canonical source of truth remains the model TSV files -- if there is any discrepancy between a field table and its source model, the model takes precedence.

For guidance on how to add or edit `//field` and `//field-via` directives in a model, see [CONTRIBUTING.md](../CONTRIBUTING.md).
