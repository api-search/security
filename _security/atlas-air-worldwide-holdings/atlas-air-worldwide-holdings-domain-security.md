---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atlasairworldwide.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atlasair.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.atlasairworldwide.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.atlasair.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.polaraircargo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atlas Air Worldwide Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas Air Worldwide Holdings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Atlas Air Worldwide Holdings
provider_slug: atlas-air-worldwide-holdings
slug: atlas-air-worldwide-holdings-domain-security
source_filename: atlas-air-worldwide-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atlasairworldwide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: www.atlasair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: www.polaraircargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: atlasairworldwide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: atlasair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas-air-worldwide-holdings/refs/heads/main/security/atlas-air-worldwide-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ACMI
- Air Cargo
- Aircraft Leasing
- Airfreight
- Airlines
- Aviation
- Charter
- CMI
- Dry Leasing
- Freight
- Freighter Operations
- Logistics
- Military Charter
- Scheduled Cargo
- Supply Chain
---
