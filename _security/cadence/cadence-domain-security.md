---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cadence.com
  spf: true
hosts:
- cert_expires: Sep 28 16:00:44 2026 GMT
  host: www.cadence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cadence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cadence Design Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cadence Design Systems
provider_slug: cadence
slug: cadence-domain-security
source_filename: cadence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cadence.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 16:00:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cadence.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadence/refs/heads/main/security/cadence-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Electronic Design Automation
- EDA
- Semiconductors
- Chip Design
- IC Design
- PCB Design
- Software
- Company
---
