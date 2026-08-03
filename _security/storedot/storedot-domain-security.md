---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: store-dot.com
  spf: true
hosts:
- cert_expires: Oct  3 05:52:36 2026 GMT
  host: www.store-dot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storedot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StoreDot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StoreDot
provider_slug: storedot
slug: storedot-domain-security
source_filename: storedot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.store-dot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:52:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: store-dot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storedot/refs/heads/main/security/storedot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Batteries
- Battery Technology
- Electric Vehicles
- Energy Storage
- Automotive
- Advanced Materials
- Clean Energy
- Manufacturing
- Nanotechnology
- Artificial Intelligence
- Israel
---
