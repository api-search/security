---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avision.io
  spf: true
hosts:
- cert_expires: Oct  5 08:29:40 2026 GMT
  host: avision.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avision
provider_slug: avision
slug: avision-domain-security
source_filename: avision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avision.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:29:40 2026 GMT\n  hsts: false\ndomains:\n- domain: avision.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avision/refs/heads/main/security/avision-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Drones
- UAS
- UTM
- U-space
- Airspace
- LAANC
- B4UFLY
- FAA
- Aviation
- Public Safety
- Advanced Air Mobility
- BVLOS
---
