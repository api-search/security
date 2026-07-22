---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: elektrikapp.com
  spf: false
hosts:
- cert_expires: Sep  4 14:33:34 2026 GMT
  host: elektrikapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elektrik App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elektrik App, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Elektrik App
provider_slug: elektrik-app
slug: elektrik-app-domain-security
source_filename: elektrik-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elektrikapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:33:34 2026 GMT\n  hsts: false\ndomains:\n- domain: elektrikapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elektrik-app/refs/heads/main/security/elektrik-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Procurement
- Medium Voltage
- Electrical Equipment
- Energy
- Supply Chain
- EPC
- Marketplace
- EnergyTech
---
