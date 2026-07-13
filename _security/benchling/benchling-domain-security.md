---
api_specs:
- filename: llms.txt
  format: yaml
  label: Benchling REST API
  slug: benchling-rest-api
  spec_type: OpenAPI
  url: https://docs.benchling.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: benchling.com
  spf: true
hosts:
- cert_expires: Oct  3 09:58:36 2026 GMT
  host: docs.benchling.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Benchling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benchling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Benchling
provider_slug: benchling
slug: benchling-domain-security
source_filename: benchling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.benchling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:58:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: benchling.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchling/refs/heads/main/security/benchling-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Biotech
- R&D
- Molecular Biology
- Laboratory Information Management
- Electronic Lab Notebook
- Assay Management
- Inventory Management
- Sequence Management
- Experiment Workflows
- REST
- Webhooks
---
