---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endurosat.com
  spf: true
hosts:
- cert_expires: Oct  5 08:18:20 2026 GMT
  host: www.endurosat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endurosat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnduroSat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EnduroSat
provider_slug: endurosat
slug: endurosat-domain-security
source_filename: endurosat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endurosat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:18:20 2026 GMT\n  hsts: false\ndomains:\n- domain: endurosat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endurosat/refs/heads/main/security/endurosat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Space
- Satellites
- CubeSat
- SmallSat
- Nanosatellites
- Ground Station
- Space Hardware
---
