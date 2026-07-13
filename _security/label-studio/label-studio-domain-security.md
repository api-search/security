---
api_specs:
- filename: label-studio-openapi.yml
  format: yaml
  label: Label Studio
  slug: label-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/label-studio/refs/heads/main/openapi/label-studio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: labelstud.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humansignal.com
  spf: true
hosts:
- cert_expires: Aug 27 19:13:51 2026 GMT
  host: labelstud.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: app.humansignal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Label Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Label Studio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Label Studio
provider_slug: label-studio
slug: label-studio-domain-security
source_filename: label-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: labelstud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.humansignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: labelstud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: humansignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/label-studio/refs/heads/main/security/label-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Annotation
- Artificial Intelligence
- Data Labeling
- LLM
- Machine Learning
- Open Source
---
