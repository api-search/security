---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sherlock.bio
  spf: true
hosts:
- cert_expires: Nov  7 16:14:14 2026 GMT
  host: sherlock.bio
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sherlock Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sherlock Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sherlock Biosciences
provider_slug: sherlock-biosciences
slug: sherlock-biosciences-domain-security
source_filename: sherlock-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sherlock.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 16:14:14 2026 GMT\n  hsts: null\ndomains:\n- domain: sherlock.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sherlock-biosciences/refs/heads/main/security/sherlock-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Diagnostics
- Molecular Diagnostics
- CRISPR
- Biotechnology
- Life Sciences
- Healthcare
- Infectious Disease
- Point of Care Testing
- Synthetic Biology
- Bioinformatics
- Acquired
---
