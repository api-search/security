---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: completeomics.com
  spf: false
hosts:
- cert_expires: Oct  4 12:13:08 2026 GMT
  host: completeomics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Completeomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complete Omics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Complete Omics
provider_slug: completeomics
slug: completeomics-domain-security
source_filename: completeomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: completeomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:13:08 2026 GMT\n  hsts: false\ndomains:\n- domain: completeomics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/completeomics/refs/heads/main/security/completeomics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Molecular Diagnostics
- Proteomics
- Multi-Omics
- Genomics
- Healthcare
- Life Sciences
- Oncology
- Companion Diagnostics
- Artificial Intelligence
---
