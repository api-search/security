---
api_specs:
- filename: university-of-illinois-urbana-champaign-rokwire-core.yaml
  format: yaml
  label: Rokwire Core Building Block
  slug: rokwire-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-rokwire-core.yaml
- filename: university-of-illinois-urbana-champaign-rokwire-gateway.yaml
  format: yaml
  label: Rokwire Gateway Building Block
  slug: rokwire-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-rokwire-gateway.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: illinois.edu
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: illinois.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: courses.illinois.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.rokwire.illinois.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Illinois Urbana Champaign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Illinois Urbana-Champaign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Illinois Urbana-Champaign
provider_slug: university-of-illinois-urbana-champaign
slug: university-of-illinois-urbana-champaign-domain-security
source_filename: university-of-illinois-urbana-champaign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: illinois.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: courses.illinois.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rokwire.illinois.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: illinois.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/security/university-of-illinois-urbana-champaign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Courses
- Library
- United States
---
