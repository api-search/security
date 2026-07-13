---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nextgen.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: meditouchehr.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.nextgen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: fhir.nextgen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: fhir.meditouchehr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nextgen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NextGen Healthcare, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NextGen Healthcare
provider_slug: api-evangelist-nextgen
slug: nextgen-domain-security
source_filename: nextgen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextgen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.nextgen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\n- host: fhir.meditouchehr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nextgen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: meditouchehr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-nextgen/refs/heads/main/security/nextgen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EHR
- FHIR
- Healthcare
- Ambulatory Care
- Clinical Data
- Patient Access
- SMART on FHIR
- Practice Management
- Interoperability
- HL7
- 21st Century Cures
---
