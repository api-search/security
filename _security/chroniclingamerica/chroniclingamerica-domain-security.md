---
api_specs:
- filename: chroniclingamerica-batches-api-openapi.yml
  format: yaml
  label: Chronicling America Batches API
  slug: chroniclingamerica-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-batches-api-openapi.yml
- filename: chroniclingamerica-issues-api-openapi.yml
  format: yaml
  label: Chronicling America Issues API
  slug: chroniclingamerica-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-issues-api-openapi.yml
- filename: chroniclingamerica-ocr-api-openapi.yml
  format: yaml
  label: Chronicling America OCR API
  slug: chroniclingamerica-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-ocr-api-openapi.yml
- filename: chroniclingamerica-pages-api-openapi.yml
  format: yaml
  label: Chronicling America Pages API
  slug: chroniclingamerica-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-pages-api-openapi.yml
- filename: chroniclingamerica-search-api-openapi.yml
  format: yaml
  label: Chronicling America Search API
  slug: chroniclingamerica-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-search-api-openapi.yml
- filename: chroniclingamerica-titles-api-openapi.yml
  format: yaml
  label: Chronicling America Titles API
  slug: chroniclingamerica-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/openapi/chroniclingamerica-titles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: loc.gov
  spf: true
hosts:
- cert_expires: Sep 13 04:56:11 2026 GMT
  host: chroniclingamerica.loc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chroniclingamerica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronicling America, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Chronicling America
provider_slug: chroniclingamerica
slug: chroniclingamerica-domain-security
source_filename: chroniclingamerica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chroniclingamerica.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:56:11 2026 GMT\n  hsts: null\ndomains:\n- domain: loc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chroniclingamerica/refs/heads/main/security/chroniclingamerica-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Newspapers
- Historical
- Archives
- Library of Congress
- Government
- Digitized
- OCR
- Search
- Cultural Heritage
---
