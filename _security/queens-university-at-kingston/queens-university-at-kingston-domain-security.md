---
api_specs:
- filename: queens-university-at-kingston-dataverse.yaml
  format: yaml
  label: Queen's University Dataverse (Borealis)
  slug: dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/queens-university-at-kingston/refs/heads/main/openapi/queens-university-at-kingston-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: queensu.ca
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: qmulus.io
  spf: true
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: www.queensu.ca
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:25:20 2026 GMT
  host: qmulus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.qmulus.io
  https: false
kind: domain-security
layout: security
method: probed
name: Queens University At Kingston Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Queen''s University at Kingston, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Queen's University at Kingston
provider_slug: queens-university-at-kingston
slug: queens-university-at-kingston-domain-security
source_filename: queens-university-at-kingston-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.queensu.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: qmulus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:25:20 2026 GMT\n  hsts: false\n- host: api.qmulus.io\n  https: false\ndomains:\n- domain: queensu.ca\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: qmulus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queens-university-at-kingston/refs/heads/main/security/queens-university-at-kingston-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research Data
- Library
- Canada
---
