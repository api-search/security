---
api_specs:
- filename: rest-api-reference.html
  format: yaml
  label: 1upHealth FHIR R4 API
  slug: 1uphealth-fhir-r4-api
  spec_type: OpenAPI
  url: https://docs.1up.health/help-center/Content/en-US/api-references/rest-api-reference.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1up.health
  spf: true
hosts:
- cert_expires: Sep  3 03:42:54 2026 GMT
  host: 1up.health
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:01:43 2026 GMT
  host: docs.1up.health
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: gateway.1up.health
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Up Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1upHealth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1upHealth
provider_slug: api-evangelist-1up-health
slug: 1up-health-domain-security
source_filename: 1up-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1up.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:42:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.1up.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:01:43 2026 GMT\n  hsts: false\n- host: gateway.1up.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 1up.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-1up-health/refs/heads/main/security/1up-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FHIR
- Health Data
- Interoperability
- Patient Access
- HL7
- SMART on FHIR
- Healthcare
- Payer
- Claims
- Electronic Prior Authorization
---
