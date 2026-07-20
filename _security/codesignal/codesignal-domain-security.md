---
api_specs:
- filename: codesignal-learn-openapi.json
  format: json
  label: CodeSignal Learn Public API
  slug: codesignal-learn-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesignal/refs/heads/main/openapi/codesignal-learn-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codesignal.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: codesignal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codesignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codesignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Codesignal
provider_slug: codesignal
slug: codesignal-domain-security
source_filename: codesignal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codesignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: codesignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesignal/refs/heads/main/security/codesignal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technical Interview
- Skills Assessment
- Hiring
- Recruiting
- Developer Skills
- Assessment
- Education
- GraphQL
- Webhooks
---
