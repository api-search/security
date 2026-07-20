---
api_specs:
- filename: kitchenstories-internal-openapi.json
  format: json
  label: Kitchen Stories Internal API
  slug: internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitchenstories/refs/heads/main/openapi/kitchenstories-internal-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kitchenstories.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kitchenstories.io
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.kitchenstories.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.kitchenstories.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.dev.kitchenstories.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitchenstories Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kitchen Stories, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kitchen Stories
provider_slug: kitchenstories
slug: kitchenstories-domain-security
source_filename: kitchenstories-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kitchenstories.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n- host: api.kitchenstories.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.dev.kitchenstories.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kitchenstories.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kitchenstories.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitchenstories/refs/heads/main/security/kitchenstories-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food and Beverage
- Recipes
- Cooking
- Media
- Content
- Consumer
- Mobile
- Video
- Germany
---
