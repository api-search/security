---
api_specs:
- filename: university-of-basel-dsp-api.yaml
  format: yaml
  label: DaSCH DSP-API
  slug: dsp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-dsp-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unibas.ch
  spf: false
hosts:
- cert_expires: Sep  7 00:46:22 2026 GMT
  host: www.unibas.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 13:31:14 2026 GMT
  host: ub.unibas.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 13:31:14 2026 GMT
  host: edoc.unibas.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Basel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Basel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: University of Basel
provider_slug: university-of-basel
slug: university-of-basel-domain-security
source_filename: university-of-basel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unibas.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ub.unibas.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:31:14 2026 GMT\n  hsts: false\n- host: edoc.unibas.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:31:14 2026 GMT\n  hsts: false\ndomains:\n- domain: unibas.ch\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/security/university-of-basel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Switzerland
- Research Data
- Open Access
- Institutional Repository
- Library
- Digital Humanities
---
