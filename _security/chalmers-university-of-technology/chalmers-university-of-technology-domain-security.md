---
api_specs:
- filename: chalmers-university-of-technology-research-api.yaml
  format: yaml
  label: Chalmers Research API
  slug: research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chalmers-university-of-technology/refs/heads/main/openapi/chalmers-university-of-technology-research-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chalmers.se
  spf: true
hosts:
- cert_expires: Sep 16 01:00:54 2026 GMT
  host: www.chalmers.se
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.research.chalmers.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: research.chalmers.se
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chalmers University Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chalmers University of Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Chalmers University of Technology
provider_slug: chalmers-university-of-technology
slug: chalmers-university-of-technology-domain-security
source_filename: chalmers-university-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chalmers.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:00:54 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.research.chalmers.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\n- host: research.chalmers.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: chalmers.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chalmers-university-of-technology/refs/heads/main/security/chalmers-university-of-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- OAI-PMH
- Sweden
---
