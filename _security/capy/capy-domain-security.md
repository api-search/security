---
api_specs:
- filename: capy-openapi-original.json
  format: json
  label: Capy API
  slug: capy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/openapi/capy-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capy.ai
  spf: true
hosts:
- cert_expires: Oct  4 08:19:27 2026 GMT
  host: capy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capy
provider_slug: capy
slug: capy-domain-security
source_filename: capy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:19:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capy.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capy/refs/heads/main/security/capy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Coding Agent
- Software Engineering
- Developer Tools
- Automation
- Code Review
- DevOps
---
