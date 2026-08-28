---
api_specs:
- filename: myome-openapi.json
  format: json
  label: MyOme API
  slug: myome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myome/refs/heads/main/openapi/myome-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myome.com
  spf: true
hosts:
- cert_expires: Oct 27 02:32:40 2026 GMT
  host: myome.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 21:08:51 2026 GMT
  host: api.myome.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 13:21:58 2026 GMT
  host: api.sbx.myome.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyOme, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MyOme
provider_slug: myome
slug: myome-domain-security
source_filename: myome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.myome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 21:08:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sbx.myome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 13:21:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myome/refs/heads/main/security/myome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Healthcare
- Clinical Laboratory
- Whole Genome Sequencing
- Precision Medicine
- Bioinformatics
- Polygenic Risk Scores
- Pharmacogenomics
- Rare Disease
- Diagnostics
- Life Sciences
---
