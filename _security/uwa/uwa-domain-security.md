---
api_specs:
- filename: uwa-research-repository.yaml
  format: yaml
  label: UWA Profiles and Research Repository (Pure CRIS Web Service)
  slug: research-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uwa/refs/heads/main/openapi/uwa-research-repository.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: uwa.edu.au
  spf: true
hosts:
- cert_expires: Oct  3 03:12:22 2026 GMT
  host: www.uwa.edu.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:12:22 2026 GMT
  host: api-portal.uwa.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 02:17:53 2026 GMT
  host: api.research-repository.uwa.edu.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uwa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Western Australia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: University of Western Australia
provider_slug: uwa
slug: uwa-domain-security
source_filename: uwa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uwa.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:12:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-portal.uwa.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:12:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.research-repository.uwa.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 02:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: uwa.edu.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uwa/refs/heads/main/security/uwa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Education
- Higher Education
- University
- Research
- Australia
- Perth
---
