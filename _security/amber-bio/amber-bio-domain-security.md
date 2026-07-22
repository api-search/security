---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amber.bio
  spf: true
hosts:
- cert_expires: Oct 15 13:12:01 2026 GMT
  host: www.amber.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amber Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amber Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amber Bio
provider_slug: amber-bio
slug: amber-bio-domain-security
source_filename: amber-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amber.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amber.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-bio/refs/heads/main/security/amber-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Engineered Biology
- RNA Editing
- Gene Editing
- Genetic Medicine
- Biotechnology
- CRISPR
- Therapeutics
---
