---
api_specs:
- filename: orbii-tech-ltd-main-openapi.json
  format: json
  label: Orbii API
  slug: orbii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-main-openapi.json
- filename: orbii-tech-ltd-ksa-openapi.json
  format: json
  label: Orbii KSA API
  slug: orbii-ksa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-ksa-openapi.json
- filename: orbii-tech-ltd-omn-openapi.json
  format: json
  label: Orbii OMN API
  slug: orbii-omn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-omn-openapi.json
- filename: orbii-tech-ltd-foodics-openapi.json
  format: json
  label: Orbii API - Foodics
  slug: orbii-api-foodics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-foodics-openapi.json
- filename: orbii-tech-ltd-rewaa-openapi.json
  format: json
  label: Orbii API - Rewaa
  slug: orbii-api-rewaa
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/openapi/orbii-tech-ltd-rewaa-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbii.ai
  spf: true
hosts:
- host: orbii.ai
  https: false
- host: api.foodics.orbii.ai
  https: false
- cert_expires: Sep 28 12:59:58 2026 GMT
  host: api.sa.orbii.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbii Tech Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbii Tech Ltd, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orbii Tech Ltd
provider_slug: orbii-tech-ltd
slug: orbii-tech-ltd-domain-security
source_filename: orbii-tech-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbii.ai\n  https: false\n- host: api.foodics.orbii.ai\n  https: false\n- host: api.sa.orbii.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:59:58 2026 GMT\n  hsts: false\ndomains:\n- domain: orbii.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii-tech-ltd/refs/heads/main/security/orbii-tech-ltd-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Lending
- Credit Scoring
- Underwriting
- Embedded Finance
- SME Finance
- Risk
- MENA
- Financial Data
---
