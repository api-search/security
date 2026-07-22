---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fromwolf.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wolf.xyz
  spf: false
hosts:
- host: fromwolf.com
  https: false
- cert_expires: Sep  1 02:55:23 2026 GMT
  host: docs.fromwolf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.wolf.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wolf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wolf, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wolf
provider_slug: wolf
slug: wolf-domain-security
source_filename: wolf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fromwolf.com\n  https: false\n- host: docs.fromwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wolf.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fromwolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wolf.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolf/refs/heads/main/security/wolf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Staffing
- Gig Economy
- Workforce Management
- Jobs
- Scheduling
- On-Demand Staffing
- Chat
---
