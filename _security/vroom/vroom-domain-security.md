---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vroom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unitedautocredit.net
  spf: true
hosts:
- cert_expires: Sep 25 20:48:05 2026 GMT
  host: www.vroom.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 14:52:53 2026 GMT
  host: www.unitedautocredit.net
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  5 14:33:27 2026 GMT
  host: www.carstory.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vroom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vroom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vroom
provider_slug: vroom
slug: vroom-domain-security
source_filename: vroom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.unitedautocredit.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 14:52:53 2026 GMT\n  hsts: true\n- host: www.carstory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 14:33:27 2026 GMT\n  hsts: false\ndomains:\n- domain: vroom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: unitedautocredit.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vroom/refs/heads/main/security/vroom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automotive
- Used Vehicles
- Vehicle Financing
- Auto Finance
- Dealer Analytics
- AI Analytics
- Non-Prime Lending
- Vehicle Inventory
---
