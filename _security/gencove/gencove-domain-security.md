---
api_specs:
- filename: gencove-openapi-original.json
  format: json
  label: Gencove Back API
  slug: gencove-back-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gencove.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: gencove.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gencove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gencove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gencove
provider_slug: gencove
slug: gencove-domain-security
source_filename: gencove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gencove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gencove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/security/gencove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Genomics
- Sequencing
- Bioinformatics
- DNA
- Life Sciences
- Analytics
---
