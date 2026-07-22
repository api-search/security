---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quibim.ai
  spf: true
hosts:
- cert_expires: Sep 14 09:21:20 2026 GMT
  host: quibim.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quibim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QUIBIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QUIBIM
provider_slug: quibim
slug: quibim-domain-security
source_filename: quibim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quibim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quibim.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quibim/refs/heads/main/security/quibim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Radiology
- Imaging Biomarkers
- Radiomics
- Life Sciences
- Drug Development
---
