---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: timely.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: timelyapp.com
  spf: true
hosts:
- cert_expires: Aug 26 03:08:01 2026 GMT
  host: www.timely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 00:23:54 2026 GMT
  host: developer.timely.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 21:31:26 2026 GMT
  host: api.timelyapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memory, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Memory
provider_slug: memory
slug: memory-domain-security
source_filename: memory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:08:01 2026 GMT\n  hsts: false\n- host: developer.timely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.timelyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:31:26 2026 GMT\n  hsts: null\ndomains:\n- domain: timely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: timelyapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memory/refs/heads/main/security/memory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Time Tracking
- Timesheets
- Productivity
- Project Management
- Professional Services
- Reporting
- Automation
- Artificial Intelligence
- SaaS
---
