---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codafication.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: unitycloud.io
  spf: true
hosts:
- cert_expires: Oct 19 14:08:30 2026 GMT
  host: codafication.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: docs.unitycloud.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codafication Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codafication, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Codafication
provider_slug: codafication
slug: codafication-domain-security
source_filename: codafication-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codafication.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 14:08:30 2026 GMT\n  hsts: false\n- host: docs.unitycloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: codafication.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: unitycloud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codafication/refs/heads/main/security/codafication-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Insurtech
- Claims
- Claims Management
- Property and Casualty
- FNOL
- Supply Chain
- GraphQL
- Webhooks
- SDK
- Extensions
- Multi Tenant
- Partner Gated
---
