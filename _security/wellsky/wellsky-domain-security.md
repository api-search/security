---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wellsky.com
  spf: true
hosts:
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: caretendapi.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.wellsky.com
  https: false
- cert_expires: Oct 15 13:02:07 2026 GMT
  host: wellsky.dynamicfhir.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wellsky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WellSky, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WellSky
provider_slug: wellsky
slug: wellsky-domain-security
source_filename: wellsky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caretendapi.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wellsky.com\n  https: false\n- host: wellsky.dynamicfhir.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 13:02:07 2026 GMT\n  hsts: null\ndomains:\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wellsky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellsky/refs/heads/main/security/wellsky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Home Health
- Hospice
- Care Coordination
- FHIR
- Clinical Documentation
- Billing
- EHR
---
