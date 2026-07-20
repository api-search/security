---
api_specs:
- filename: exec-openapi-original.yml
  format: yaml
  label: Exec API
  slug: exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/openapi/exec-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exec.com
  spf: true
hosts:
- cert_expires: Aug 31 11:27:00 2026 GMT
  host: api.exec.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exec
provider_slug: exec
slug: exec-domain-security
source_filename: exec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.exec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:27:00 2026 GMT\n  hsts: null\ndomains:\n- domain: exec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exec/refs/heads/main/security/exec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Training
- Roleplay
- Coaching
- Learning
- Knowledge Management
- LMS
---
