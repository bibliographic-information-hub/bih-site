# BIH Site

This repository is the top-level home for **Bibliographic Information Hub (BIH)** resources.

It is intended to back the top-level BIH landing page and the resources exposed under `w3id.org/bih/`.

The main application template currently lives at:

- <https://github.com/bibliographic-information-hub/bih-app>

At this stage, `bih-site` is the place for:

- BIH overview and landing-page content
- shared ontology and schema resources
- stable top-level links to the app template and example instances

## Repository Structure

- `ontology/`
  Shared BIH ontology resources.
- `schema/`
  Public JSON Schema resources used by BIH applications and instances.
- `index.html`
  A redirecting language entry point for the top-level BIH site.
- `en/`
  English landing-page content.
- `ja/`
  Japanese landing-page content.

## Related Repositories

- `bibliographic-information-hub/bih-app`
  The reusable BIH application template.
- `cm3`-side fork / instance repositories such as `bih-cm3`
  Example issuer-specific BIH instances with real collections and items.

## Current Resources

- [BIH entry schema](./schema/bih-entry.schema.json)
- [BIH properties ontology](./ontology/bih-properties.ttl)

## Publishing Intention

The top-level BIH web presence should explain:

- what BIH is
- the core BIH concepts
- how BIH is structured across issuer, collection, and item
- where the ontology, schemas, and software live
- how to publish a BIH instance of your own

This repository is therefore not only for ontology files, but also for human-facing landing-page content.

English is currently the primary documentation language here. Japanese content can be added separately later.

The top-level `/` entry point can redirect by explicit query parameter such as `?lang=en` or `?lang=ja`, and otherwise
falls back to a stored preference or the browser language.
