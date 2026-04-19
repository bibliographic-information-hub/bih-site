# BIH Site Development Notes

## Language Policy

- The top-level BIH landing site currently maintains English and Japanese entry pages.
- English is treated as the primary outward-facing documentation language for broader accessibility.
- Japanese is provided as a parallel page set rather than as inline mixed-language content.
- The top-level `/` entry point may redirect to a preferred language based on `?lang=en` / `?lang=ja`, stored preference, or browser language.
- Direct links for language switching should point to explicit paths such as `/en/` and `/ja/`, not to the redirecting top-level `/`.
- If additional languages are added later, they should normally follow the same explicit-path pattern.

## Top-Level Content Scope

- The public landing pages should focus on outward-facing explanation, core concepts, and links to the main repositories and resources.
- Repository-internal explanations such as what this repository is meant to hold over time should live here in `DEVELOPMENT.md`, not on the public landing page itself.
- In practice, `bih-site` is intended to hold:
  - top-level explanation of the BIH model
  - shared ontology and schema files
  - links to the app template and public BIH instances
  - future guidance for publishers who want to run their own BIH deployment
