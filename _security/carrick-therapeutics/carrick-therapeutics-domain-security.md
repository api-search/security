---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carricktherapeutics.com
  spf: true
hosts:
- cert_expires: Aug 26 08:05:19 2026 GMT
  host: carricktherapeutics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carrick Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carrick Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Carrick Therapeutics
provider_slug: carrick-therapeutics
slug: carrick-therapeutics-domain-security
source_filename: carrick-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carricktherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:05:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carricktherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrick-therapeutics/refs/heads/main/security/carrick-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Oncology
- Clinical Stage
- Drug Development
---
