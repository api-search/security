---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clearcareonline.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wellsky.com
  spf: true
hosts:
- cert_expires: Aug  6 13:35:23 2026 GMT
  host: www.clearcareonline.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 04:37:12 2026 GMT
  host: wellsky.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearCare, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ClearCare
provider_slug: clearcare
slug: clearcare-domain-security
source_filename: clearcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearcareonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 13:35:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: wellsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:37:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clearcareonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wellsky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearcare/refs/heads/main/security/clearcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Home Care
- Home Health
- Healthcare
- Agency Management
- Caregiving
- Electronic Visit Verification
- SaaS
- Scheduling
---
