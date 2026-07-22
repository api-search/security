---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firstgrid.cn
  spf: false
hosts:
- cert_expires: Aug  5 23:59:59 2026 GMT
  host: www.firstgrid.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Firstgrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for firstgrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: firstgrid
provider_slug: firstgrid
slug: firstgrid-domain-security
source_filename: firstgrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstgrid.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: firstgrid.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstgrid/refs/heads/main/security/firstgrid-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Medical Devices
- Supply Chain
- Logistics
- Healthcare
- Software
- China
---
