---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crystaldynamics.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: crystaldynamics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crystal Dynamics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crystal Dynamics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Crystal Dynamics
provider_slug: crystal-dynamics
slug: crystal-dynamics-domain-security
source_filename: crystal-dynamics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crystaldynamics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: crystaldynamics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crystal-dynamics/refs/heads/main/security/crystal-dynamics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Video Games
- Game Studio
- Entertainment
- Media
---
