---
api_specs:
- filename: tetrascience-openapi.yml
  format: yaml
  label: Tetra Scientific Data and AI Cloud API
  slug: tetra-data-and-ai-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrascience/refs/heads/main/openapi/tetrascience-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tetrascience.com
  spf: true
hosts:
- cert_expires: Aug 24 01:54:39 2026 GMT
  host: www.tetrascience.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:44:44 2026 GMT
  host: developers.tetrascience.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: api.tetrascience.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tetrascience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TetraScience, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TetraScience
provider_slug: tetrascience
slug: tetrascience-domain-security
source_filename: tetrascience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tetrascience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:54:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.tetrascience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:44:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tetrascience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tetrascience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tetrascience/refs/heads/main/security/tetrascience-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scientific Data
- Life Sciences
- Pharma
- Biotech
- Lab Data
- Lab Automation
- Data Platform
- Data Engineering
- AI Platform
- Scientific AI
- FAIR Data
- GxP Compliance
- Chromatography
- Spectroscopy
- Cloud Data Lake
- Pipelines
- Agents
- IDS
---
