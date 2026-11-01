---
api_specs:
- filename: youlearn-openapi-generated.yml
  format: yaml
  label: YouLearn API
  slug: youlearn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/youlearn/openapi/_ae-authored/youlearn-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: youlearn.ai
  spf: true
hosts:
- cert_expires: Dec 25 02:21:14 2026 GMT
  host: youlearn.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Youlearn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YouLearn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: YouLearn
provider_slug: youlearn
slug: youlearn-domain-security
source_filename: youlearn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: youlearn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 02:21:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: youlearn.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/youlearn/security/youlearn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- AI
- Tutoring
- Learning
---
