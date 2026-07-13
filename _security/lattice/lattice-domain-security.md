---
api_specs:
- filename: lattice-talent-openapi.yml
  format: yaml
  label: Lattice Talent API
  slug: lattice-talent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-talent-openapi.yml
- filename: lattice-hris-openapi.yml
  format: yaml
  label: Lattice HRIS API
  slug: lattice-hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-hris-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lattice.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: latticehq.com
  spf: true
hosts:
- cert_expires: Sep  3 06:52:58 2026 GMT
  host: lattice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:48:40 2026 GMT
  host: developers.lattice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:25 2026 GMT
  host: api.latticehq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lattice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lattice, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lattice
provider_slug: lattice
slug: lattice-domain-security
source_filename: lattice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lattice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:52:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.lattice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.latticehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:25 2026 GMT\n  hsts: false\ndomains:\n- domain: lattice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: latticehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/security/lattice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- People Management
- Performance Management
- OKRs
- Goals
- Employee Engagement
- HRIS
- Compensation
- Feedback
- Surveys
---
