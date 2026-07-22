---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kestrl.io
  spf: true
hosts:
- cert_expires: Sep 13 04:06:20 2026 GMT
  host: kestrl.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kestrl Muslim Money App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kestrl: Muslim Money App, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 'Kestrl: Muslim Money App'
provider_slug: kestrl-muslim-money-app
slug: kestrl-muslim-money-app-domain-security
source_filename: kestrl-muslim-money-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kestrl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:06:20 2026 GMT\n  hsts: null\ndomains:\n- domain: kestrl.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kestrl-muslim-money-app/refs/heads/main/security/kestrl-muslim-money-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Islamic Finance
- Ethical Banking
- Personal Finance
- Mobile Banking
- Payments
- Techstars
---
