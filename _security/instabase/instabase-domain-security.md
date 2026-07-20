---
api_specs:
- filename: instabase-aihub-openapi.yaml
  format: yaml
  label: Instabase AI Hub API
  slug: instabase-ai-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instabase/refs/heads/main/openapi/instabase-aihub-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instabase.com
  spf: true
hosts:
- cert_expires: Oct  6 02:38:59 2026 GMT
  host: www.instabase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: aihub.instabase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instabase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instabase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instabase
provider_slug: instabase
slug: instabase-domain-security
source_filename: instabase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:38:59 2026 GMT\n  hsts: false\n- host: aihub.instabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabase/refs/heads/main/security/instabase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Intelligent Document Processing
- Document AI
- Artificial Intelligence
- Machine Learning
- Automation
- Data Extraction
- LLM
- Financial Services
- Insurance
---
