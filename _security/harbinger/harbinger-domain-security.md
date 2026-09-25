---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harbingermotors.com
  spf: true
hosts:
- cert_expires: Sep 29 02:44:36 2026 GMT
  host: harbingermotors.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Harbinger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harbinger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harbinger
provider_slug: harbinger
slug: harbinger-domain-security
source_filename: harbinger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harbingermotors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:44:36 2026 GMT\n  hsts: false\ndomains:\n- domain: harbingermotors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/security/harbinger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Electric Vehicles
- Commercial Vehicles
- Medium Duty Trucks
- Manufacturing
- Fleet Management
- Transportation
- Logistics
- Energy Storage
---
