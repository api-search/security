---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: timeisltd.com
  spf: true
hosts:
- cert_expires: Oct  9 03:00:50 2026 GMT
  host: www.timeisltd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Time Is Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Time is Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Time is Ltd
provider_slug: time-is-ltd
slug: time-is-ltd-domain-security
source_filename: time-is-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timeisltd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:00:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: timeisltd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/time-is-ltd/refs/heads/main/security/time-is-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Analytics
- Collaboration
- Productivity
- People Analytics
- SaaS
---
