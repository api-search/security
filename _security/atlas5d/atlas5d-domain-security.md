---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atlas5d.com
  spf: true
hosts:
- cert_expires: Sep 29 21:11:33 2026 GMT
  host: atlas5d.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atlas5D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas5D, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Atlas5D
provider_slug: atlas5d
slug: atlas5d-domain-security
source_filename: atlas5d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atlas5d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:11:33 2026 GMT\n  hsts: false\ndomains:\n- domain: atlas5d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas5d/refs/heads/main/security/atlas5d-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Health Technology
- Remote Patient Monitoring
- Ambient Computing
- Sensors
- Aging in Place
- Clinical Trials
- Digital Health
---
