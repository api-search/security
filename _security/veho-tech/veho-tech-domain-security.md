---
api_specs:
- filename: veho-tech-api-openapi-original.yml
  format: yaml
  label: Veho API
  slug: veho-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veho-tech/refs/heads/main/openapi/veho-tech-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipveho.com
  spf: true
hosts:
- cert_expires: Sep 20 00:03:10 2026 GMT
  host: www.shipveho.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 20:44:25 2026 GMT
  host: docs.api.shipveho.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.shipveho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veho Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veho Tech, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Veho Tech
provider_slug: veho-tech
slug: veho-tech-domain-security
source_filename: veho-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipveho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:03:10 2026 GMT\n  hsts: false\n- host: docs.api.shipveho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:44:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.shipveho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shipveho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veho-tech/refs/heads/main/security/veho-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Shipping
- Last-Mile Delivery
- Package Tracking
- E-Commerce
- Delivery
- Webhooks
---
