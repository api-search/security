---
api_specs:
- filename: depop-selling-openapi-original.yml
  format: yaml
  label: Depop Selling API
  slug: depop-selling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depop/refs/heads/main/openapi/depop-selling-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: depop.com
  spf: true
hosts:
- cert_expires: Oct  4 16:44:08 2026 GMT
  host: www.depop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Depop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for depop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: depop
provider_slug: depop
slug: depop-domain-security
source_filename: depop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.depop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:44:08 2026 GMT\n  hsts: null\ndomains:\n- domain: depop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depop/refs/heads/main/security/depop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fashion
- Marketplace
- E-commerce
- Resale
- Retail
- Inventory Management
- Orders
- Sustainability
---
