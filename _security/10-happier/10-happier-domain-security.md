---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tenpercent.com
  spf: true
hosts:
- cert_expires: Oct 15 10:41:32 2026 GMT
  host: www.tenpercent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 10 Happier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 10% Happier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 10% Happier
provider_slug: 10-happier
slug: 10-happier-domain-security
source_filename: 10-happier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tenpercent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:41:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tenpercent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/10-happier/refs/heads/main/security/10-happier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Meditation
- Mindfulness
- Wellness
- Mobile App
- Health
---
