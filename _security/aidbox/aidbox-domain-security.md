---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: health-samurai.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: aidbox.app
  spf: false
hosts:
- cert_expires: Oct  1 05:15:33 2026 GMT
  host: www.health-samurai.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 10:30:20 2026 GMT
  host: sandbox.aidbox.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aidbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aidbox, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aidbox
provider_slug: aidbox
slug: aidbox-domain-security
source_filename: aidbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.health-samurai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:15:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.aidbox.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:30:20 2026 GMT\n  hsts: null\ndomains:\n- domain: health-samurai.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aidbox.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidbox/refs/heads/main/security/aidbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- EHR
- Health Data
- FHIR Server
- Bulk Data
- Terminology
- Digital Health
---
