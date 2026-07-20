---
api_specs:
- filename: astronomer-astro-openapi-original.yml
  format: yaml
  label: Astro Platform API
  slug: astro-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-astro-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astronomer.io
  spf: true
hosts:
- cert_expires: Sep 25 11:54:04 2026 GMT
  host: astronomer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 11:54:04 2026 GMT
  host: www.astronomer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.astronomer.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astronomer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astronomer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astronomer
provider_slug: astronomer
slug: astronomer-domain-security
source_filename: astronomer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astronomer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.astronomer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.astronomer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: astronomer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/security/astronomer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Orchestration
- Apache Airflow
- Data Pipelines
- Data Engineering
- Workflow Automation
- MLOps
- Managed Platform
---
