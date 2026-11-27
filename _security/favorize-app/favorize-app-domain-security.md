---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: favorize.app
  spf: true
hosts:
- cert_expires: Dec 21 20:14:06 2026 GMT
  host: favorize.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Favorize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Favorize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Favorize
provider_slug: favorize-app
slug: favorize-app-domain-security
source_filename: favorize-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: favorize.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 20:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: favorize.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/favorize-app/security/favorize-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wishlist
- E-Commerce
- Artificial Intelligence
- Privacy
- Collaboration
---
