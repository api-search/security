---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: airtime.com
  spf: true
hosts:
- cert_expires: Sep 29 17:40:30 2026 GMT
  host: airtime.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airtime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airtime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Airtime
provider_slug: airtime
slug: airtime-domain-security
source_filename: airtime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airtime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:40:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: airtime.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtime/refs/heads/main/security/airtime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Video
- Productivity
- Collaboration
- Screen Recording
- Presentations
- Remote Work
---
