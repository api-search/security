---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: purism-ev.com
  spf: false
hosts:
- cert_expires: Oct  7 03:03:02 2026 GMT
  host: purism-ev.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purismev Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PurismEV Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: PurismEV Inc.
provider_slug: purismev-inc
slug: purismev-inc-domain-security
source_filename: purismev-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: purism-ev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:03:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: purism-ev.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purismev-inc/refs/heads/main/security/purismev-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Electric Vehicles
- Energy Management
- Fleet Management
- Battery
- Automotive
- Mobility
- Sustainability
---
