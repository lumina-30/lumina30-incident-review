# L30-FRM Code System for Claude Review

This file summarizes the document ID, filename, and localization system used in this review package.

## Core rule

`L30-FRM-B01`, `L30-FRM-B02`, `L30-FRM-I01`, `L30-FRM-I02`, `L30-FRM-I03`, `L30-FRM-A01`, `L30-FRM-G01`, `L30-FRM-R01`, and `L30-FRM-S01` are the current official document IDs. Document IDs use hyphens; public filenames use underscores.

English files are the canonical templates and do not use a language suffix.

Localized files use an uppercase language suffix immediately before the file extension.

Japanese files use the `_JA` suffix.

Language suffixes such as `_JA`, `_FR`, or `_DE` are not part of the document ID.

## Official document IDs

```text
L30-FRM-B01 = Boundary_Check
L30-FRM-B02 = Operational_Refusal_Preservation_Minimum
L30-FRM-I01 = Incident_Review_Template
L30-FRM-I02 = Incident_Review_Protocol
L30-FRM-I03 = Incident_Review_Protocol_Extended
L30-FRM-A01 = Audit_Checklist
L30-FRM-G01 = Governance_Review_Template
L30-FRM-R01 = Responsibility_Accountability_Review
L30-FRM-S01 = Stabilization_Checklist
```

## Filename rule

Public filenames continue to use `L30_FRM_` with underscores for filesystem and URL compatibility.

## Language-specific files

```text
L30_FRM_B01_Boundary_Check.docx
L30_FRM_B01_Boundary_Check_JA.docx
L30_FRM_B01_Boundary_Check_FR.docx
```

## Localization rule

Localized versions should be created by copying the English canonical template and translating only the human-readable text.

Document IDs, L30-BAS codes, field structure, checkbox controls, tables, code placement, and layout should be preserved across localized versions.

Japanese localized versions may be provided as reference examples for localization. They are not required for every supporting or detailed form unless the form is intended for Japanese-language practical use.

## Review focus

Please check that:

- the package treats `L30-FRM-*` as document IDs;
- English files are treated as canonical files without a language suffix;
- localized files use uppercase language suffixes only as filename suffixes;
- Japanese files use `_JA`, not `_JP`;
- no language suffix is treated as part of the document ID;
- no underscored `L30_FRM_*` value remains in DocID fields;
- no filename uses spaces;
- form bodies do not show language code as part of the document ID;
- Markdown links point to existing DOCX/PDF files;
- the forms do not present themselves as certification, legal approval, or substitutes for PCR-C or the LUMINA-30 Boundary Kernel.

## Stable public filenames

Public filenames do not include version numbers. The English form is the default filename. Localized forms use uppercase language suffixes before the file extension.
