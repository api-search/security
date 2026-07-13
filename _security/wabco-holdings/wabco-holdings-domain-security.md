---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wabco-holdings.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wabco-solutioncentre.com
  spf: true
hosts:
- host: www.wabco-holdings.com
  https: false
- cert_expires: Sep 30 14:02:03 2026 GMT
  host: wabco-solutioncentre.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- host: api.wabco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Wabco Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WABCO Holdings, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WABCO Holdings
provider_slug: wabco-holdings
slug: wabco-holdings-domain-security
source_filename: wabco-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wabco-holdings.com\n  https: false\n- host: wabco-solutioncentre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.wabco.com\n  https: false\ndomains:\n- domain: wabco-holdings.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: wabco-solutioncentre.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wabco-holdings/refs/heads/main/security/wabco-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Vehicles
- Fleet Management
- Telematics
- Safety Systems
- Transportation
- Fortune 1000
---
