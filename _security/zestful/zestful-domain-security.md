---
api_specs:
- filename: zestful-openapi.yml
  format: yaml
  label: Zestful Ingredient Parser API
  slug: zestful
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zestful/refs/heads/main/openapi/zestful-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zestfuldata.com
  spf: true
hosts:
- cert_expires: Aug 15 22:44:15 2026 GMT
  host: zestfuldata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:22:57 2026 GMT
  host: sandbox.zestfuldata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zestful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zestful, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zestful
provider_slug: zestful
slug: zestful-domain-security
source_filename: zestful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zestfuldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 22:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.zestfuldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:22:57 2026 GMT\n  hsts: null\ndomains:\n- domain: zestfuldata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zestful/refs/heads/main/security/zestful-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Food
- Ingredients
- Parsers
- Recipes
- USDA
---
