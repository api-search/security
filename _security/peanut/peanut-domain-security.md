---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: peanut-app.io
  spf: true
hosts:
- cert_expires: Sep 20 19:02:26 2026 GMT
  host: www.peanut-app.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peanut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peanut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Peanut
provider_slug: peanut
slug: peanut-domain-security
source_filename: peanut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peanut-app.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:02:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peanut-app.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peanut/refs/heads/main/security/peanut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Network
- Women
- Motherhood
- Fertility
- Pregnancy
- Menopause
- Community
- Mobile App
---
