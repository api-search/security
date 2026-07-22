---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inductive.bio
  spf: true
hosts:
- cert_expires: Sep  4 02:09:34 2026 GMT
  host: www.inductive.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inductive Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inductive Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inductive Bio
provider_slug: inductive-bio
slug: inductive-bio-domain-security
source_filename: inductive-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inductive.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:09:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inductive.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inductive-bio/refs/heads/main/security/inductive-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Drug Discovery
- Machine Learning
- Artificial Intelligence
- ADMET
- Small Molecule
- Computational Chemistry
- Life Sciences
- Biotech
- Pharmaceuticals
---
