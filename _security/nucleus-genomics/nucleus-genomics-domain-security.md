---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mynucleus.com
  spf: true
hosts:
- cert_expires: Nov  1 15:55:11 2026 GMT
  host: mynucleus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nucleus Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nucleus Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nucleus Genomics
provider_slug: nucleus-genomics
slug: nucleus-genomics-domain-security
source_filename: nucleus-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mynucleus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:55:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mynucleus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nucleus-genomics/refs/heads/main/security/nucleus-genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Health
- Consumer Genetics
- Whole Genome Sequencing
- Fertility
- IVF
- Carrier Screening
- Precision Medicine
- Biotechnology
---
