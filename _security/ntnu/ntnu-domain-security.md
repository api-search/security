---
api_specs:
- filename: ntnu-dataverseno.yaml
  format: yaml
  label: DataverseNO Research Data API
  slug: dataverseno
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntnu/refs/heads/main/openapi/ntnu-dataverseno.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ntnu.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: cristin.no
  spf: false
hosts:
- cert_expires: Dec 21 01:29:06 2026 GMT
  host: www.ntnu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 13:34:51 2026 GMT
  host: api.cristin.no
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: nva.sikt.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ntnu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norwegian University of Science and Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Norwegian University of Science and Technology
provider_slug: ntnu
slug: ntnu-domain-security
source_filename: ntnu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ntnu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 01:29:06 2026 GMT\n  hsts: false\n- host: api.cristin.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 13:34:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: nva.sikt.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ntnu.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cristin.no\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntnu/refs/heads/main/security/ntnu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Norway
- Scandinavia
---
