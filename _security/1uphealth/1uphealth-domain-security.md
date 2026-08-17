---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1up.health
  spf: true
hosts:
- cert_expires: Nov  1 11:49:55 2026 GMT
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
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: api.1up.health
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Uphealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1upHealth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1upHealth
provider_slug: 1uphealth
slug: 1uphealth-domain-security
source_filename: 1uphealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1up.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 11:49:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.1up.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:01:43 2026 GMT\n  hsts: false\n- host: api.1up.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 1up.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1uphealth/refs/heads/main/security/1uphealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Payer
- Claims
- Patient Access
- Health Data
---
