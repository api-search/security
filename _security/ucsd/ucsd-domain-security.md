---
api_specs:
- filename: ucsd-tritonai.yaml
  format: yaml
  label: TritonAI Developer API
  slug: tritonai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-tritonai.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ucsd.edu
  spf: true
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: www.ucsd.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: developer.ucsd.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: collab.ucsd.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ucsd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, San Diego, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of California, San Diego
provider_slug: ucsd
slug: ucsd-domain-security
source_filename: ucsd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucsd.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: false\n- host: developer.ucsd.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: false\n- host: collab.ucsd.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ucsd.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/security/ucsd-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United States
- California
---
