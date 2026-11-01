---
api_specs:
- filename: thehive-ai-task-api-openapi.yml
  format: yaml
  label: Hive Task API
  slug: thehive-ai-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thehive-ai/openapi/thehive-ai-task-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thehive.ai
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: thehive.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thehive Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hive
provider_slug: thehive-ai
slug: thehive-ai-domain-security
source_filename: thehive-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thehive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thehive.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thehive-ai/security/thehive-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Machine Learning
- Data Labeling
- Enterprise
---
