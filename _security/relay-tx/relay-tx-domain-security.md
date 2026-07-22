---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: relaytx.com
  spf: true
hosts:
- cert_expires: Sep 23 17:29:30 2026 GMT
  host: relaytx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relay Tx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relay Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Relay Therapeutics
provider_slug: relay-tx
slug: relay-tx-domain-security
source_filename: relay-tx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relaytx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:29:30 2026 GMT\n  hsts: false\ndomains:\n- domain: relaytx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relay-tx/refs/heads/main/security/relay-tx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Drug Discovery
- Precision Medicine
- Oncology
- Genetic Disease
- Protein Motion
- Computational Chemistry
- Molecular Dynamics
- Cryo-EM
- Machine Learning
- DNA-Encoded Libraries
- Allosteric Inhibitors
- PI3K-Alpha
- NRAS
- FGFR2
- Fabry Disease
- Biotechnology
- Clinical Stage
---
