---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datakrew.com
  spf: true
hosts:
- cert_expires: Aug 30 04:17:07 2026 GMT
  host: datakrew.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datakrew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datakrew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datakrew
provider_slug: datakrew
slug: datakrew-domain-security
source_filename: datakrew-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datakrew.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 04:17:07 2026 GMT\n  hsts: null\ndomains:\n- domain: datakrew.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datakrew/refs/heads/main/security/datakrew-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Mobility
- Electric Vehicles
- Battery Intelligence
- Fleet Management
- Telematics
- IoT
- Artificial Intelligence
- Logistics
- Transportation
---
