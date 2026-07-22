---
api_specs:
- filename: wefitter-openapi-original.json
  format: json
  label: WeFitter API
  slug: wefitter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/openapi/wefitter-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:caa@wftr.nl"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: wefitter.com
  spf: true
hosts:
- cert_expires: Oct  6 21:04:01 2026 GMT
  host: wefitter.com
  hsts: true
  hsts_max_age: 63082000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:02:56 2026 GMT
  host: api.wefitter.com
  hsts: true
  hsts_max_age: 63082000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wefitter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeFitter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: WeFitter
provider_slug: wefitter
slug: wefitter-domain-security
source_filename: wefitter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wefitter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:04:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63082000\n- host: api.wefitter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:02:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63082000\ndomains:\n- domain: wefitter.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:caa@wftr.nl\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wefitter/refs/heads/main/security/wefitter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Fitness
- Wearables
- Health Data
- Wellbeing
- Gamification
- Digital Health
- Insurance
- Activity Tracking
---
