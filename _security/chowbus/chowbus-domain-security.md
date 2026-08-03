---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chowbus.com
  spf: true
hosts:
- cert_expires: Sep 30 00:17:12 2026 GMT
  host: www.chowbus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 04:37:15 2026 GMT
  host: pos.chowbus.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: merchant dashboard SPA; host added manually during the 2026-08-02 enrichment pass (not reachable from apis.yml Website alone)
  tls_version: TLSv1.3
- cert_expires: Oct  8 04:37:15 2026 GMT
  host: pos-api.chowbus.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: live JSON API host, undocumented
  tls_version: TLSv1.3
- cert_expires: Oct  8 04:37:15 2026 GMT
  host: api.chowbus.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: legacy marketplace-era Rails backend
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chowbus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chowbus, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chowbus
provider_slug: chowbus
slug: chowbus-domain-security
source_filename: chowbus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chowbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pos.chowbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: merchant dashboard SPA; host added manually during the 2026-08-02 enrichment\n    pass (not reachable from apis.yml Website alone)\n- host: pos-api.chowbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: live JSON API host, undocumented\n- host: api.chowbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note:\
  \ legacy marketplace-era Rails backend\ndomains:\n- domain: chowbus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chowbus/refs/heads/main/security/chowbus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Restaurants
- Point of Sale
- Restaurant Technology
- Food and Beverage
- Online Ordering
- Payments
- Loyalty
- Hospitality
- SaaS
- Artificial Intelligence
- United States
---
