---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seurat.com
  spf: true
hosts:
- cert_expires: Sep  2 11:52:40 2026 GMT
  host: www.seurat.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seurat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seurat Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seurat Technologies
provider_slug: seurat
slug: seurat-domain-security
source_filename: seurat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seurat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 11:52:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: seurat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seurat/refs/heads/main/security/seurat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Metal Manufacturing
- Contract Manufacturing
- Industrial
- Aerospace
- Automotive
- Defense
- Reshoring
---
