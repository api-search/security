---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: loftdynamics.com
  spf: true
hosts:
- cert_expires: Sep 25 22:17:48 2026 GMT
  host: loftdynamics.com
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loft Dynamics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loft Dynamics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Loft Dynamics
provider_slug: loft-dynamics
slug: loft-dynamics-domain-security
source_filename: loft-dynamics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loftdynamics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:17:48 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: loftdynamics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loft-dynamics/refs/heads/main/security/loft-dynamics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Aviation
- Flight Simulation
- Virtual Reality
- Pilot Training
- Simulation
---
