---
api_specs:
- filename: melorra-catalog-api-openapi.yml
  format: yaml
  label: Melorra Catalog API
  slug: melorra-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/openapi/melorra-catalog-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: melorra.com
  spf: true
hosts:
- cert_expires: Dec  3 14:17:38 2026 GMT
  host: www.melorra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 14:17:38 2026 GMT
  host: services-catalog.melorra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Melorra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melorra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Melorra
provider_slug: melorra
slug: melorra-domain-security
source_filename: melorra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.melorra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 14:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: services-catalog.melorra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 14:17:38 2026 GMT\n  hsts: null\ndomains:\n- domain: melorra.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melorra/refs/heads/main/security/melorra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Jewellery
- Retail
- E-Commerce
- Product Catalog
- Direct to Consumer
- Fashion
- India
---
