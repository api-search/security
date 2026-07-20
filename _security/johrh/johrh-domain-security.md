---
api_specs:
- filename: johrh-openapi.json
  format: json
  label: Johrh Storefront (Zid Vitrin)
  slug: johrh-storefront-zid-vitrin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johrh/refs/heads/main/openapi/johrh-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: johrh.com
  spf: true
hosts:
- cert_expires: Sep 15 14:16:40 2026 GMT
  host: johrh.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Johrh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Johrh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Johrh
provider_slug: johrh
slug: johrh-domain-security
source_filename: johrh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: johrh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:16:40 2026 GMT\n  hsts: null\ndomains:\n- domain: johrh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johrh/refs/heads/main/security/johrh-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Retail
- E-commerce
- Fashion
- Apparel
- Abaya
- Modest Wear
- Saudi Arabia
- Zid
- Storefront
---
