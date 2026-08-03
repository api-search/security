---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rapidai.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rapid-sys.com
  spf: false
hosts:
- cert_expires: Sep  9 05:19:13 2026 GMT
  host: www.rapidai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.us.rapid-sys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapidai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RapidAI, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RapidAI
provider_slug: rapidai
slug: rapidai-domain-security
source_filename: rapidai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rapidai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.us.rapid-sys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rapidai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rapid-sys.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidai/refs/heads/main/security/rapidai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Radiology
- Clinical Decision Support
- Stroke
- DICOM
- HL7
- FHIR
- Diagnostics
---
