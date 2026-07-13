---
api_specs:
- filename: asyncapi.yml
  format: yaml
  label: Gumroad v2 API
  slug: v2-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumroad/refs/heads/main/asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gumroad.com
  spf: true
hosts:
- cert_expires: Sep  6 19:50:19 2026 GMT
  host: gumroad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 19:50:19 2026 GMT
  host: app.gumroad.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 19:50:19 2026 GMT
  host: api.gumroad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gumroad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gumroad, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gumroad
provider_slug: gumroad
slug: gumroad-domain-security
source_filename: gumroad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gumroad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:50:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.gumroad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:50:19 2026 GMT\n  hsts: false\n- host: api.gumroad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:50:19 2026 GMT\n  hsts: null\ndomains:\n- domain: gumroad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumroad/refs/heads/main/security/gumroad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Commerce
- Creator Economy
- Digital Products
- Memberships
- License Keys
- Affiliates
- E-commerce
---
