---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ucar.edu
  spf: true
hosts:
- cert_expires: Dec  7 22:33:42 2026 GMT
  host: www.ucar.edu
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Corporation For Atmospheric Research Ucar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University Corporation for Atmospheric Research (UCAR), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University Corporation for Atmospheric Research (UCAR)
provider_slug: university-corporation-for-atmospheric-research-ucar
slug: university-corporation-for-atmospheric-research-ucar-domain-security
source_filename: university-corporation-for-atmospheric-research-ucar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucar.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 22:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: ucar.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/university-corporation-for-atmospheric-research-ucar/security/university-corporation-for-atmospheric-research-ucar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Research
- AtmosphericScience
- Education
- Nonprofit
---
