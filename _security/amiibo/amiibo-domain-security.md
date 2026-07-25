---
api_specs:
- filename: amiibo-amiibo-api-openapi.yml
  format: yaml
  label: Amiibo API Amiibo API
  slug: amiibo-amiibo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amiibo/refs/heads/main/openapi/amiibo-amiibo-api-openapi.yml
- filename: amiibo-metadata-api-openapi.yml
  format: yaml
  label: Amiibo API Metadata API
  slug: amiibo-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amiibo/refs/heads/main/openapi/amiibo-metadata-api-openapi.yml
- filename: amiibo-reference-api-openapi.yml
  format: yaml
  label: Amiibo API Reference API
  slug: amiibo-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amiibo/refs/heads/main/openapi/amiibo-reference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amiiboapi.org
  spf: true
hosts:
- host: amiiboapi.org
  https: false
kind: domain-security
layout: security
method: probed
name: Amiibo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amiibo API, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Amiibo API
provider_slug: amiibo
slug: amiibo-domain-security
source_filename: amiibo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amiiboapi.org\n  https: false\ndomains:\n- domain: amiiboapi.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amiibo/refs/heads/main/security/amiibo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Nintendo
- Amiibo
- Gaming
- Figures
- Characters
- Video Games
- REST
---
