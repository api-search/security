---
api_specs:
- filename: brandfetch-brand-api.yml
  format: yaml
  label: Brandfetch Brand API
  slug: brandfetch-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brandfetch-brand-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: brandfetch.com
  spf: true
hosts:
- cert_expires: Sep 20 05:24:51 2026 GMT
  host: docs.brandfetch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brand Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brand API (Brandfetch), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brand API (Brandfetch)
provider_slug: brand-api
slug: brand-api-domain-security
source_filename: brand-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.brandfetch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:24:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brandfetch.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/security/brand-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Brands
- Logos
- Brand Assets
- Company Data
- Firmographics
---
