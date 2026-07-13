---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arubanetworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hpe.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.arubanetworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: www.hpe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: devhub.arubanetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aruba Hpe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HPE Aruba Networking, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HPE Aruba Networking
provider_slug: aruba-hpe
slug: aruba-hpe-domain-security
source_filename: aruba-hpe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arubanetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\n- host: www.hpe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: null\n- host: devhub.arubanetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: arubanetworks.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hpe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aruba-hpe/refs/heads/main/security/aruba-hpe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Networking
- Switching
- Wi-Fi
- SD-WAN
- NAC
- Network Access Control
- Cloud Networking
- AIOps
- Data Center
- Campus
- Branch
- Edge
- SSE
- SASE
- HPE
---
