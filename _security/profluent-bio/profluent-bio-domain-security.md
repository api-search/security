---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: profluent.bio
  spf: true
hosts:
- cert_expires: Sep 17 05:01:23 2026 GMT
  host: www.profluent.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Profluent Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Profluent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Profluent
provider_slug: profluent-bio
slug: profluent-bio-domain-security
source_filename: profluent-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.profluent.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:01:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: profluent.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profluent-bio/refs/heads/main/security/profluent-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Protein Design
- Protein Language Models
- Foundation Models
- Generative Biology
- Gene Editing
- CRISPR
- OpenCRISPR
- ProGen
- ProseLM
- Bioinformatics
- Therapeutics
- Agriculture
- Industrial Enzymes
- Open Source Models
---
