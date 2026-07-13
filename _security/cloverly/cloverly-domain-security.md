---
api_specs:
- filename: cloverly-estimates-api-openapi.yml
  format: yaml
  label: Cloverly Estimates API
  slug: cloverly-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-estimates-api-openapi.yml
- filename: cloverly-purchases-api-openapi.yml
  format: yaml
  label: Cloverly Purchases API
  slug: cloverly-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-purchases-api-openapi.yml
- filename: cloverly-offset-types-api-openapi.yml
  format: yaml
  label: Cloverly Offset Types API
  slug: cloverly-offset-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-offset-types-api-openapi.yml
- filename: cloverly-account-api-openapi.yml
  format: yaml
  label: Cloverly Account API
  slug: cloverly-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/openapi/cloverly-account-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cloverly.com
  spf: true
hosts:
- cert_expires: Sep 10 23:39:53 2026 GMT
  host: cloverly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 22:14:44 2026 GMT
  host: docs.cloverly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 17:42:39 2026 GMT
  host: api.cloverly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloverly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloverly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cloverly
provider_slug: cloverly
slug: cloverly-domain-security
source_filename: cloverly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloverly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloverly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloverly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:42:39 2026 GMT\n  hsts: false\ndomains:\n- domain: cloverly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverly/refs/heads/main/security/cloverly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Carbon
- Carbon Credits
- Carbon Offsets
- Catalyst
- Climate
- Climate Action
- Climate Impact X
- CIX
- Decarbonization
- ESG
- Greenhouse Gas
- Net Zero
- Project Developers
- Registries
- Sustainability
- Voluntary Carbon Market
- VCM
---
