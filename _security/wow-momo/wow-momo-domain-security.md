---
api_specs:
- filename: wow-momo-content-api-openapi.yml
  format: yaml
  label: WOW! Momo Content API
  slug: wow-momo-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wow-momo/refs/heads/main/openapi/_ae-authored/wow-momo-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wowmomo.com
  spf: true
hosts:
- cert_expires: Oct  4 23:49:32 2026 GMT
  host: www.wowmomo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.wowmomo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wow Momo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WOW! Momo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WOW! Momo
provider_slug: wow-momo
slug: wow-momo-domain-security
source_filename: wow-momo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wowmomo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:49:32 2026 GMT\n  hsts: false\n- host: api.wowmomo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wowmomo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wow-momo/refs/heads/main/security/wow-momo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurants
- Food and Beverage
- Quick Service Restaurant
- Retail
- Hospitality
- Consumer
- Franchising
- Content
- WordPress
- oEmbed
- India
- Kolkata
---
