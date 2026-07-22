---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: propetroservices.com
  spf: true
hosts:
- cert_expires: Sep 24 23:21:18 2026 GMT
  host: www.propetroservices.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propetro Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProPetro Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ProPetro Holding
provider_slug: propetro-holding
slug: propetro-holding-domain-security
source_filename: propetro-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propetroservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:21:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: propetroservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propetro-holding/refs/heads/main/security/propetro-holding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Fortune 1000
- Oil and Gas
- Oilfield Services
- Hydraulic Fracturing
- Permian Basin
---
