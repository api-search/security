---
api_specs:
- filename: purdue-catalog.yaml
  format: yaml
  label: Purdue.io Course Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-catalog.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: purdue.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: purdue.io
  spf: false
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.purdue.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:39:01 2026 GMT
  host: api.purdue.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 13:59:15 2026 GMT
  host: purr.purdue.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purdue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Purdue University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Purdue University
provider_slug: purdue
slug: purdue-domain-security
source_filename: purdue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.purdue.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.purdue.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:39:01 2026 GMT\n  hsts: false\n- host: purr.purdue.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: purdue.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: purdue.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/security/purdue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United States
---
