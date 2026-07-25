---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tempus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tempus.ai
  spf: true
hosts:
- cert_expires: Oct 20 16:16:03 2026 GMT
  host: www.tempus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 02:49:39 2026 GMT
  host: lens.tempus.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tempus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tempus, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tempus
provider_slug: tempus
slug: tempus-domain-security
source_filename: tempus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tempus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 16:16:03 2026 GMT\n  hsts: null\n- host: lens.tempus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:49:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tempus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tempus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tempus/refs/heads/main/security/tempus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- Genomics
- Precision Medicine
- Clinical AI
- Oncology
- FHIR
- HL7
- EHR
- Interoperability
- Life Sciences
- Real-World Data
---
