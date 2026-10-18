---
api_specs:
- filename: conveyor-single-question-api-openapi.yml
  format: yaml
  label: Conveyor Single Question API
  slug: conveyor-single-question-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conveyor/refs/heads/main/openapi/conveyor-single-question-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conveyor.com
  spf: true
hosts:
- cert_expires: Nov 27 06:25:13 2026 GMT
  host: www.conveyor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conveyor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conveyor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Conveyor
provider_slug: conveyor
slug: conveyor-domain-security
source_filename: conveyor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conveyor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 06:25:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conveyor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conveyor/refs/heads/main/security/conveyor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Security Questionnaire Automation
- RFP Automation
- Trust Center
- Customer Trust
- Compliance
- Knowledge Management
---
