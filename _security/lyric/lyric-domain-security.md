---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lyric.tech
  spf: true
hosts:
- cert_expires: Oct 14 15:03:25 2026 GMT
  host: lyric.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lyric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lyric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lyric
provider_slug: lyric
slug: lyric-domain-security
source_filename: lyric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lyric.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:03:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lyric.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyric/refs/heads/main/security/lyric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Supply Chain
- Logistics
- Artificial Intelligence
- Optimization
- Forecasting
- Enterprise Software
---
