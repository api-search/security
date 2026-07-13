---
api_specs:
- filename: taylors-library-rest.yaml
  format: yaml
  label: Taylor's Library Koha REST API
  slug: library-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-library-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taylors.edu.my
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: university.taylors.edu.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: librarycatalogue.taylors.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: irepo.taylors.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Taylors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taylor''s University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taylor's University
provider_slug: taylors
slug: taylors-domain-security
source_filename: taylors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: university.taylors.edu.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: librarycatalogue.taylors.edu.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\n- host: irepo.taylors.edu.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: taylors.edu.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/security/taylors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Library
- Institutional Repository
- Open Data
- Malaysia
- Asia
---
