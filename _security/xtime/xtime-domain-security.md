---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xtime.com
  spf: true
hosts:
- cert_expires: Sep 27 06:21:34 2026 GMT
  host: xtime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xtime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xtime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xtime
provider_slug: xtime
slug: xtime-domain-security
source_filename: xtime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xtime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:21:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xtime.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xtime/refs/heads/main/security/xtime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Software
- Automotive
- Dealerships
- Service Scheduling
- Vehicle Inspection
- Customer Engagement
- Fixed Operations
---
