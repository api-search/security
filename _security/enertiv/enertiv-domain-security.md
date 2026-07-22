---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enertiv.com
  spf: true
hosts:
- host: enertiv.com
  https: false
  note: apex returns a TLS internal-error alert; canonical host is www.enertiv.com
- host: www.enertiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- host: app.enertiv.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: nginx
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Enertiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enertiv, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enertiv
provider_slug: enertiv
slug: enertiv-domain-security
source_filename: enertiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml website + subdomains\nhosts:\n- host: enertiv.com\n  https: false\n  note: apex returns a TLS internal-error alert; canonical host is www.enertiv.com\n- host: www.enertiv.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  server: cloudflare\n- host: app.enertiv.com\n  https: true\n  tls_version: TLSv1.2\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: nginx\ndomains:\n- domain: enertiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enertiv/refs/heads/main/security/enertiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- PropTech
- Sustainability
- ESG
- Energy Management
- Decarbonization
- Building Operations
- Utility Billing
- Predictive Maintenance
---
