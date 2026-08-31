---
api_specs:
- filename: brand-api-brands-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Brands API
  slug: brand-api-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-brands-api-openapi.yml
- filename: brand-api-context-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Context API
  slug: brand-api-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-context-api-openapi.yml
- filename: brand-api-search-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Search API
  slug: brand-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-search-api-openapi.yml
- filename: brand-api-viewer-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Viewer API
  slug: brand-api-viewer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-viewer-api-openapi.yml
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Brand Api Trust Center
name_suffix: Trust Center
overview: Brand API (Brandfetch) maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Brand API (Brandfetch)
provider_slug: brand-api
slug: brand-api-trust-center
source_filename: brand-api-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://docs.brandfetch.com/support/security-soc2\nurl: https://trust.brandfetch.com\nplatform: Vanta\ncertifications:\n  - SOC 2 Type 2\nscope:\n  trust_service_categories: [Security]\n  note: >-\n    The independent audit covers the Security trust service category only. Availability,\n    Confidentiality, Processing Integrity and Privacy are not claimed.\npractices:\n  data_minimization: >-\n    Brandfetch states it collects no PII beyond login email addresses used for\n    passwordless authentication.\n  log_retention: 'Up to 90 days; may include IP addresses and User-Agent strings.'\n  data_scope: >-\n    The API processes only publicly available data tied to domain names and does not\n    access, store or interact with private or customer-owned data.\n  encryption: 'AES-256 at rest, TLS in transit.'\n  hosting: 'Amazon Web Services (development, staging and production).'\n  sdlc: 'OWASP best practices with\
  \ human review augmented by AI.'\nevidence:\n  - source: https://docs.brandfetch.com/support/security-soc2\n    http_status: 200\n    keywords: ['SOC 2 Type 2', 'Trust Center', 'AES-256', 'OWASP', 'AWS']\n    quote: >-\n      \"Brandfetch is SOC 2 Type 2 certified. You can access our report and security\n      documentation at our Trust Center.\"\n  - source: https://trust.brandfetch.com\n    http_status: 200\n    note: >-\n      Vanta-hosted trust report. The page is client-rendered, so the certification list\n      is not readable from the raw HTML — only the title \"Brandfetch Trust Center\" and the\n      Vanta asset manifest are. The certification recorded above is taken from\n      Brandfetch's own docs page, not inferred from this shell. The automated\n      probe-security-programs.py pass returned trust=none for exactly this reason.\nnote: >-\n  Requesting the SOC 2 report itself requires accepting an NDA through the Vanta portal;\n  the report was not retrieved and is not asserted\
  \ beyond Brandfetch's own published claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/security/brand-api-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Brands
- Logos
- Brand Assets
- Company Data
- Firmographics
- Brand Context
- Merchant Enrichment
- Agent Tools
trust_url: https://trust.brandfetch.com
---
