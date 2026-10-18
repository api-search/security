---
api_specs:
- filename: cobot2-openapi.yml
  format: yaml
  label: Cobot API
  slug: cobot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobot2/refs/heads/main/openapi/cobot2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cobot.me
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.cobot.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cobot2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobot2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cobot2
provider_slug: cobot2
slug: cobot2-domain-security
source_filename: cobot2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cobot.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cobot.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobot2/refs/heads/main/security/cobot2-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Co-Working
- Software-as-a-Service
- Management
- Software
- Collaboration
- Company
---
