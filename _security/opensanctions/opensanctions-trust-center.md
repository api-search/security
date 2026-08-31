---
api_specs:
- filename: opensanctions-api-openapi.yml
  format: yaml
  label: OpenSanctions Screening API
  slug: opensanctions-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensanctions/refs/heads/main/openapi/opensanctions-api-openapi.yml
certifications:
- ISO/IEC 27001:2022
description: ''
kind: trust-center
layout: security
name: Opensanctions Trust Center
name_suffix: Trust Center
overview: OpenSanctions maintains a public trust center documenting ISO/IEC 27001:2022 compliance.
provider_name: OpenSanctions
provider_slug: opensanctions
slug: opensanctions-trust-center
source_filename: opensanctions-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nprobe: true\nurl: https://trust.opensanctions.org/\nvendor: Vanta\ncertifications:\n  - ISO/IEC 27001:2022\nauditor: Consilium Labs\nevidence:\n  - source: https://trust.opensanctions.org/\n    status: 200\n    keywords: [trust center]\n    note: >-\n      Confirmed to be a Vanta-hosted trust center from the asset host\n      (assets.vanta.com) in the served HTML. The page renders client-side: the\n      HTML body contains 28 characters of text (\"OpenSanctions Trust Center\") and\n      nothing else, so no certification, sub-processor or control list is readable\n      without executing JavaScript.\n  - source: https://www.opensanctions.org/docs/security/\n    status: 200\n    keywords: [ISO/IEC 27001:2022, Consilium Labs, security@opensanctions.org]\n    note: >-\n      The certification claim is taken from this server-rendered page rather than\n      the trust center, and names the certifying body.\nlinked_from:\n  - https://www.opensanctions.org/docs/opensource/\
  \ (footer, \"Trust Center\")\n  - https://www.opensanctions.org/llms.txt (\"Vendor information\")\nnot_found:\n  - SOC 2\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - CSA STAR\n  - published sub-processor list\nnote: >-\n  Absence above means \"not readable on the surfaces probed\", not \"does not exist\" —\n  the Vanta portal may list more behind its JS render.\nx-evidence:\n  fetched: '2026-08-27'\n  probes:\n    - {url: 'https://trust.opensanctions.org/', status: 200}\n    - {url: 'https://www.opensanctions.org/docs/security/', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensanctions/refs/heads/main/security/opensanctions-trust-center.yml
summary_line: ISO/IEC 27001:2022
tags:
- Sanctions Screening
- Anti-Money Laundering
- Politically Exposed Persons
- Compliance
- Financial Crime
- Know Your Customer
- Entity Resolution
- Open Data
- Risk Data
- Due Diligence
- Public APIs
- agent-native
trust_url: https://trust.opensanctions.org/
---
