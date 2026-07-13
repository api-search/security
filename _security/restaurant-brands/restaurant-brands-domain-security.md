---
api_specs:
- filename: channel-openapi.yml
  format: yaml
  label: Channel Partners API
  slug: channel-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/openapi/channel-openapi.yml
- filename: menu-v2-openapi.yml
  format: yaml
  label: Partners Menu API v2
  slug: partners-menu-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/openapi/menu-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rbi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rbictg.com
  spf: false
hosts:
- cert_expires: Aug 19 02:30:59 2026 GMT
  host: www.rbi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: bk-partners.rbictg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: sandbox-bk-partners.rbictg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restaurant Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restaurant Brands International, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Restaurant Brands International
provider_slug: restaurant-brands
slug: restaurant-brands-domain-security
source_filename: restaurant-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rbi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:30:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bk-partners.rbictg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: sandbox-bk-partners.rbictg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: rbi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rbictg.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/security/restaurant-brands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Franchising
- Hospitality
- NYSE QSR
- Quick Service Restaurants
- Restaurants
---
