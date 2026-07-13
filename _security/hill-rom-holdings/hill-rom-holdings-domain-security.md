---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hillrom.com
  spf: true
hosts:
- cert_expires: Nov  6 21:23:10 2026 GMT
  host: www.hillrom.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hill Rom Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hill-Rom Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hill-Rom Holdings
provider_slug: hill-rom-holdings
slug: hill-rom-holdings-domain-security
source_filename: hill-rom-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hillrom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 21:23:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: hillrom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hill-rom-holdings/refs/heads/main/security/hill-rom-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Devices
- Hospital Beds
- Patient Monitoring
- Vital Signs
- Connected Care
- Cardiac Diagnostics
---
