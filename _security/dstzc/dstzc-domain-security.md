---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: dstcar.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: www.dstcar.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dstzc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dstzc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: dstzc
provider_slug: dstzc
slug: dstzc-domain-security
source_filename: dstzc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dstcar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dstcar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dstzc/refs/heads/main/security/dstzc-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Logistics
- Electric Vehicles
- Fleet Management
- New Energy
- Transportation
- Mobility
- China
---
