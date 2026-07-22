---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biotree.cn
  spf: true
hosts:
- cert_expires: Nov 12 07:18:22 2026 GMT
  host: biotree.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biotree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biotree, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Biotree
provider_slug: biotree
slug: biotree-domain-security
source_filename: biotree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biotree.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:18:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biotree.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biotree/refs/heads/main/security/biotree-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Life Sciences
- Metabolomics
- Proteomics
- Multi-Omics
- Mass Spectrometry
- Biotechnology
- CDMO
---
