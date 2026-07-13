---
api_specs:
- filename: m3ter-openapi.yml
  format: yaml
  label: M3ter API
  slug: m3ter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/m3ter/refs/heads/main/openapi/m3ter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: m3ter.com
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: www.m3ter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.m3ter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M3Ter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M3ter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: M3ter
provider_slug: m3ter
slug: m3ter-domain-security
source_filename: m3ter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.m3ter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.m3ter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: m3ter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m3ter/refs/heads/main/security/m3ter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinOps
- Usage-Based Billing
- Metering
- Billing
- Pricing
- SaaS
---
