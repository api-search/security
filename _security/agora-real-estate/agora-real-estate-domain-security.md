---
api_specs:
- filename: agora-real-estate-o-embed-api-openapi.yml
  format: yaml
  label: Agora Real Estate o Embed API
  slug: agora-real-estate-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-o-embed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agorareal.com
  spf: true
hosts:
- cert_expires: Nov 22 12:16:07 2026 GMT
  host: agorareal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 01:36:44 2026 GMT
  host: websiteapi.agorareal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 17:02:08 2026 GMT
  host: auth.agorareal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agora Real Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agora Real Estate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agora Real Estate
provider_slug: agora-real-estate
slug: agora-real-estate-domain-security
source_filename: agora-real-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agorareal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 12:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: websiteapi.agorareal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 01:36:44 2026 GMT\n  hsts: false\n- host: auth.agorareal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 17:02:08 2026 GMT\n  hsts: false\ndomains:\n- domain: agorareal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/security/agora-real-estate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Investment Management
- Private Equity
- Fund Administration
- Investor Relations
- Capital Raising
- Syndication
- Fund Accounting
- Investor Portal
- CRM
- Payments
- Content Management
- Software-as-a-Service
---
