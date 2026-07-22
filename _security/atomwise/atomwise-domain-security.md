---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atomwise.com
  spf: true
hosts:
- cert_expires: Sep  6 18:25:43 2026 GMT
  host: www.atomwise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomwise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atomwise
provider_slug: atomwise
slug: atomwise-domain-security
source_filename: atomwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atomwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:25:43 2026 GMT\n  hsts: false\ndomains:\n- domain: atomwise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomwise/refs/heads/main/security/atomwise-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Drug Discovery
- Biotech
- Pharmaceuticals
- Structure-Based Drug Design
- Virtual Screening
- Deep Learning
- Convolutional Neural Networks
- AtomNet
- Small Molecules
- Cheminformatics
- AIMS Program
- Numerion Labs
---
