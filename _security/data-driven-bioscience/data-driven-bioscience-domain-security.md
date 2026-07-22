---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: datadrivenbioscience.com
  spf: true
hosts:
- cert_expires: Aug 25 12:03:28 2026 GMT
  host: datadrivenbioscience.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Driven Bioscience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Driven Bioscience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Data Driven Bioscience
provider_slug: data-driven-bioscience
slug: data-driven-bioscience-domain-security
source_filename: data-driven-bioscience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datadrivenbioscience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:03:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: datadrivenbioscience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-driven-bioscience/refs/heads/main/security/data-driven-bioscience-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Genomics
- Oncology
- Diagnostics
- Life Sciences
- Bioinformatics
---
