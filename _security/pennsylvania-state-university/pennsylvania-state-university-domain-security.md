---
api_specs:
- filename: pennsylvania-state-university-fis.yaml
  format: yaml
  label: LionSpaceFIS REST API
  slug: fis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/openapi/pennsylvania-state-university-fis.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: psu.edu
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.psu.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: apps.opp.psu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: metadata.libraries.psu.edu
  hsts: true
  hsts_max_age: 30
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pennsylvania State University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pennsylvania State University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pennsylvania State University
provider_slug: pennsylvania-state-university
slug: pennsylvania-state-university-domain-security
source_filename: pennsylvania-state-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.psu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apps.opp.psu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\n- host: metadata.libraries.psu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 30\ndomains:\n- domain: psu.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennsylvania-state-university/refs/heads/main/security/pennsylvania-state-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Facilities
- United States
---
