---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: littlespoon.com
  spf: true
hosts:
- cert_expires: Oct  7 18:42:48 2026 GMT
  host: www.littlespoon.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:42:48 2026 GMT
  host: api.littlespoon.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 7776000
  https: true
  note: 'Undocumented first-party JSON API host, fronted by Cloudflare over a Heroku router (via: 2.0 heroku-router). Probed 2026-08-25.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Little Spoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Little Spoon, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Little Spoon
provider_slug: little-spoon
slug: little-spoon-domain-security
source_filename: little-spoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the littlespoon.com web host and the api.littlespoon.com API host\nhosts:\n- host: www.littlespoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: api.littlespoon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains: true\n  note: >-\n    Undocumented first-party JSON API host, fronted by Cloudflare over a Heroku router\n    (via: 2.0 heroku-router). Probed 2026-08-25.\ndomains:\n- domain: littlespoon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes:\n- No CAA record is published on littlespoon.com, so certificate issuance is not constrained to a\n  named CA.\n- DNSSEC is not enabled on littlespoon.com.\n- DMARC policy is p=quarantine rather than p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/little-spoon/refs/heads/main/security/little-spoon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Consumer Products
- E-Commerce
- Subscription
- Direct to Consumer
- Baby Food
- Nutrition
- Retail
- Design System
---
