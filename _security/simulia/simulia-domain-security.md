---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 3ds.com
  spf: true
hosts:
- cert_expires: Sep  5 20:33:46 2026 GMT
  host: www.3ds.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simulia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SIMULIA (Dassault Systemes), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SIMULIA (Dassault Systemes)
provider_slug: simulia
slug: simulia-domain-security
source_filename: simulia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3ds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: 3ds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simulia/refs/heads/main/security/simulia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Simulation
- FEA
- CFD
- Electromagnetics
- Optimization
- Engineering
- Dassault Systemes
- 3DEXPERIENCE
---
