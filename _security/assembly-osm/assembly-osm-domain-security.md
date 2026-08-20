---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: assemblyosm.com
  spf: true
hosts:
- cert_expires: Sep 28 04:17:08 2026 GMT
  host: www.assemblyosm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assembly Osm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assembly OSM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Assembly OSM
provider_slug: assembly-osm
slug: assembly-osm-domain-security
source_filename: assembly-osm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.assemblyosm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: assemblyosm.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assembly-osm/refs/heads/main/security/assembly-osm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Construction
- Modular Construction
- Off-Site Manufacturing
- Prefabrication
- Real-Estate
- Housing
- Architecture
- Digital Twin
- Sustainability
- Climate Tech
- Manufacturing
- New York
---
