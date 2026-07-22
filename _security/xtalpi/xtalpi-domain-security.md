---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xtalpi.com
  spf: true
hosts:
- cert_expires: Aug 30 05:30:48 2026 GMT
  host: en.xtalpi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xtalpi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XtalPi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: XtalPi
provider_slug: xtalpi
slug: xtalpi-domain-security
source_filename: xtalpi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.xtalpi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 05:30:48 2026 GMT\n  hsts: false\ndomains:\n- domain: xtalpi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xtalpi/refs/heads/main/security/xtalpi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Drug Discovery
- Pharmaceutical Research
- AI Drug Discovery
- Quantum Mechanics
- Quantum Physics
- Computational Chemistry
- Generative Chemistry
- Molecular Simulation
- Free Energy Perturbation
- Solid-State Research
- Peptide Therapeutics
- Lab Automation
- Intelligent Laboratories
- Robotics
- Materials Science
- Life Sciences
- Biotechnology
---
