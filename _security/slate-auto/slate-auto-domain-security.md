---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slate.auto
  spf: true
hosts:
- cert_expires: Sep  2 01:34:25 2026 GMT
  host: www.slate.auto
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slate Auto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slate Auto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slate Auto
provider_slug: slate-auto
slug: slate-auto-domain-security
source_filename: slate-auto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slate.auto\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:34:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: slate.auto\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slate-auto/refs/heads/main/security/slate-auto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electric Vehicles
- Automotive
- EV
- Electric Truck
- Manufacturing
- Mobility
- Fleet
- Customization
- Consumer
---
