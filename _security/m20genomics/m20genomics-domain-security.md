---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: m20genomics.com
  spf: true
hosts:
- cert_expires: Sep  6 06:11:50 2026 GMT
  host: m20genomics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M20Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M20 Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: M20 Genomics
provider_slug: m20genomics
slug: m20genomics-domain-security
source_filename: m20genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: m20genomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:11:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: m20genomics.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m20genomics/refs/heads/main/security/m20genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Genomics
- Life Sciences
- Single-Cell Sequencing
- Spatial Transcriptomics
- Bioinformatics
- Biotechnology
---
