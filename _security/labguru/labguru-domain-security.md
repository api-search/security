---
api_specs:
- filename: labguru-rest-api-v1.yaml
  format: yaml
  label: Labguru REST API
  slug: labguru-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labguru/refs/heads/main/openapi/labguru-rest-api-v1.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: labguru.com
  spf: true
hosts:
- cert_expires: Sep 14 22:31:03 2026 GMT
  host: www.labguru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: my.labguru.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labguru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labguru, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Labguru
provider_slug: labguru
slug: labguru-domain-security
source_filename: labguru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.labguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:31:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.labguru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: labguru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labguru/refs/heads/main/security/labguru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electronic Lab Notebook
- ELN
- LIMS
- Laboratory Information Management
- Biotech
- Life Sciences
- Research Data Management
- Inventory Management
- Experiment Management
- REST API
- GraphQL
---
