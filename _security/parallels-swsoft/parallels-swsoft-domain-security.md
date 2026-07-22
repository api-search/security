---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parallels.com
  spf: true
hosts:
- cert_expires: Oct 13 01:29:56 2026 GMT
  host: www.parallels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parallels Swsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallels (SWSoft), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parallels (SWSoft)
provider_slug: parallels-swsoft
slug: parallels-swsoft-domain-security
source_filename: parallels-swsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parallels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:29:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parallels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallels-swsoft/refs/heads/main/security/parallels-swsoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Virtualization
- Remote Desktop
- Application Delivery
- Cloud Infrastructure
- VDI
- Automation
- REST API
---
