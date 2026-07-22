---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: schrodinger.com
  spf: true
hosts:
- cert_expires: Sep 21 07:14:36 2026 GMT
  host: www.schrodinger.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 05:50:09 2026 GMT
  host: my.schrodinger.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schrodinger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schrödinger, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Schrödinger
provider_slug: schrodinger
slug: schrodinger-domain-security
source_filename: schrodinger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.schrodinger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:14:36 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: my.schrodinger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:50:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: schrodinger.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schrodinger/refs/heads/main/security/schrodinger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drug Discovery
- Computational Chemistry
- Molecular Simulation
- Physics-Based Modeling
- Free Energy Perturbation
- Molecular Dynamics
- Quantum Chemistry
- Materials Science
- Biologics
- Cheminformatics
- AI for Science
- Life Sciences
- Pharmaceuticals
- Maestro
- LiveDesign
- PyMOL
- Python API
- KNIME
- Enterprise Software
- Public Company
---
