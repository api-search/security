---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyperganic.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: hyperganic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperganic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperganic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hyperganic
provider_slug: hyperganic
slug: hyperganic-domain-security
source_filename: hyperganic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyperganic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hyperganic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperganic/refs/heads/main/security/hyperganic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Tech
- Additive Manufacturing
- 3D Printing
- Generative Design
- Algorithmic Engineering
- Simulation
- Computational Design
---
