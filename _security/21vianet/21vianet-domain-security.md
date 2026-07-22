---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 21vianet.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vnet.com
  spf: true
hosts:
- host: www.21vianet.com
  https: false
- cert_expires: Sep 25 06:33:47 2026 GMT
  host: www.vnet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 21Vianet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 21Vianet, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 21Vianet
provider_slug: 21vianet
slug: 21vianet-domain-security
source_filename: 21vianet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.21vianet.com\n  https: false\n- host: www.vnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 21vianet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: vnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/21vianet/refs/heads/main/security/21vianet-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Infrastructure
- Data Center
- Cloud
- Hosting
- Colocation
- China
- Managed Services
---
