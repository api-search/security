---
api_specs:
- filename: stacker-openapi.yml
  format: yaml
  label: Stacker API
  slug: stacker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacker/refs/heads/main/openapi/stacker-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stacker.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stackerhq.com
  spf: true
hosts:
- cert_expires: Aug 23 19:23:02 2026 GMT
  host: stacker.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 00:13:41 2026 GMT
  host: docs.stackerhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 21:34:44 2026 GMT
  host: api.go.stackerhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stacker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stacker, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stacker
provider_slug: stacker
slug: stacker-domain-security
source_filename: stacker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stacker.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:23:02 2026 GMT\n  hsts: false\n- host: docs.stackerhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.go.stackerhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:34:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stacker.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stackerhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacker/refs/heads/main/security/stacker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Development
- Low-Code
- No-Code
- Portals
- Workflow Automation
---
