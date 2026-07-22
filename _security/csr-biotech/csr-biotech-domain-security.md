---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: csr-biotech.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: csr-biotech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Csr Biotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CSR Biotech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CSR Biotech
provider_slug: csr-biotech
slug: csr-biotech-domain-security
source_filename: csr-biotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csr-biotech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: csr-biotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csr-biotech/refs/heads/main/security/csr-biotech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Microscopy
- Super-Resolution Imaging
- Life Sciences
- Scientific Instruments
- Biotechnology
---
