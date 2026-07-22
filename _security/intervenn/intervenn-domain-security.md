---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intervenn.com
  spf: true
hosts:
- cert_expires: Sep 23 01:03:59 2026 GMT
  host: intervenn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intervenn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InterVenn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: InterVenn
provider_slug: intervenn
slug: intervenn-domain-security
source_filename: intervenn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intervenn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:03:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intervenn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intervenn/refs/heads/main/security/intervenn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Digital Biology
- Glycoproteomics
- Proteomics
- Mass Spectrometry
- Precision Medicine
- Biomarkers
- Artificial Intelligence
- Life Sciences
---
