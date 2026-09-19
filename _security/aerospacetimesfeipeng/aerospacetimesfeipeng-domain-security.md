---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: htsdfp.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.htsdfp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aerospacetimesfeipeng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerospace Times Feipeng, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Aerospace Times Feipeng
provider_slug: aerospacetimesfeipeng
slug: aerospacetimesfeipeng-domain-security
source_filename: aerospacetimesfeipeng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.htsdfp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: htsdfp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerospacetimesfeipeng/refs/heads/main/security/aerospacetimesfeipeng-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Company
- Aerospace
- Drones
- UAV
- Logistics
- Manufacturing
- Aviation
- Low Altitude Economy
- China
---
