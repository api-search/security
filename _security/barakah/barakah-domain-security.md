---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: barakah.app
  spf: true
hosts:
- cert_expires: Oct  4 23:32:43 2026 GMT
  host: barakah.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barakah Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barakah, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Barakah
provider_slug: barakah
slug: barakah-domain-security
source_filename: barakah-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barakah.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: barakah.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barakah/refs/heads/main/security/barakah-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food Tech
- Food Waste
- Sustainability
- Marketplace
- Mobile App
- Saudi Arabia
- Food Delivery
---
