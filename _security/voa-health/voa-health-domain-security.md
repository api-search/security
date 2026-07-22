---
api_specs:
- filename: voa-health-rnds-openapi.yml
  format: yaml
  label: Voa RNDS Integration API
  slug: voa-rnds-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voa-health/refs/heads/main/openapi/voa-health-rnds-openapi.yml
- filename: voa-health-identify-openapi.yml
  format: yaml
  label: Voa Integration Identify API
  slug: voa-integration-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voa-health/refs/heads/main/openapi/voa-health-identify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voa.health
  spf: true
hosts:
- cert_expires: Aug 19 21:31:24 2026 GMT
  host: voa.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voa Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VOA Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VOA Health
provider_slug: voa-health
slug: voa-health-domain-security
source_filename: voa-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voa.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:31:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: voa.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voa-health/refs/heads/main/security/voa-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Clinical Documentation
- EHR
- FHIR
- RNDS
- Artificial Intelligence
- Brazil
---
