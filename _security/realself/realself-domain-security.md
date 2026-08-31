---
api_specs:
- filename: realself-lead-sharing-asyncapi.yml
  format: yaml
  label: RealSelf Lead Sharing
  slug: realself-lead-sharing
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realself/refs/heads/main/asyncapi/realself-lead-sharing-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: realself.com
  spf: true
hosts:
- cert_expires: Mar 22 20:00:19 2027 GMT
  host: www.realself.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.realself.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realself Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealSelf, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RealSelf
provider_slug: realself
slug: realself-domain-security
source_filename: realself-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realself.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 22 20:00:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.realself.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: realself.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realself/refs/heads/main/security/realself-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Healthcare
- Aesthetics
- Marketplace
- Reviews
- Lead Generation
- Consumer Health
- Webhook
- JSON-Schema
---
