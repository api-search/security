---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: timelyapp.com
  spf: true
hosts:
- cert_expires: Dec  1 18:18:07 2026 GMT
  host: timelyapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Timely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timely (Memory AS), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Timely (Memory AS)
provider_slug: timely
slug: timely-domain-security
source_filename: timely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: timelyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 18:18:07 2026 GMT\n  hsts: false\ndomains:\n- domain: timelyapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/timely/security/timely-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Time Tracking
- AI
- SaaS
- Productivity
---
