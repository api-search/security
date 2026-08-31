---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: immunitastx.com
  spf: true
hosts:
- cert_expires: Oct  2 16:02:08 2026 GMT
  host: www.immunitastx.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Immunitas Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immunitas Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Immunitas Therapeutics
provider_slug: immunitas-therapeutics
slug: immunitas-therapeutics-domain-security
source_filename: immunitas-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.immunitastx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: immunitastx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immunitas-therapeutics/refs/heads/main/security/immunitas-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Therapeutics
- Oncology
- Immunology
- Autoimmune Disease
- Single Cell Analysis
- Spatial Transcriptomics
- Bioinformatics
- Open-Source
- Life Sciences
---
