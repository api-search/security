---
api_specs:
- filename: advance-auto-parts-catalog-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Catalog API
  slug: advance-auto-parts-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-catalog-api-openapi.yml
- filename: advance-auto-parts-commerce-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Commerce API
  slug: advance-auto-parts-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-commerce-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: advanceautoparts.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.advanceautoparts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.advanceautoparts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Advance Auto Parts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advance Auto Parts, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
slug: advance-auto-parts-domain-security
source_filename: advance-auto-parts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.advanceautoparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.advanceautoparts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: advanceautoparts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/security/advance-auto-parts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
- Fortune 500
---
