---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iceonline.cn
  spf: false
hosts:
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: www.iceonline.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Iceonline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iceonline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: iceonline
provider_slug: iceonline
slug: iceonline-domain-security
source_filename: iceonline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iceonline.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: iceonline.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iceonline/refs/heads/main/security/iceonline-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Ice Rink
- Facility Management
- Enterprise Software
- Sports and Recreation
- SaaS
- China
---
