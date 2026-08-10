---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bit.bio
  spf: true
hosts:
- cert_expires: Sep 22 13:02:38 2026 GMT
  host: www.bit.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bit.Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bit.bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bit.bio
provider_slug: bit.bio
slug: bit.bio-domain-security
source_filename: bit.bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bit.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:02:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bit.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bit.bio/refs/heads/main/security/bit.bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Synthetic Biology
- Biotechnology
- Life Sciences
- Stem Cells
- Cell Therapy
- Drug Discovery
- Genomics
- CRISPR
- Research Reagents
---
