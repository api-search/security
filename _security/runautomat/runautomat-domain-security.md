---
api_specs:
- filename: runautomat-extract-openapi.json
  format: json
  label: Automat Document Extraction API
  slug: automat-document-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runautomat/refs/heads/main/openapi/runautomat-extract-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: runautomat.com
  spf: true
hosts:
- cert_expires: Oct 11 16:12:38 2026 GMT
  host: runautomat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runautomat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runautomat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Runautomat
provider_slug: runautomat
slug: runautomat-domain-security
source_filename: runautomat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runautomat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:12:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: runautomat.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runautomat/refs/heads/main/security/runautomat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Automation
- Robotic Process Automation
- Document Processing
- Artificial Intelligence
- Machine Learning
- Data Extraction
- iPaaS
- Agents
---
