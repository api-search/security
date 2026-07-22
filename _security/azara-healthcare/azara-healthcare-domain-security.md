---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azarahealthcare.com
  spf: true
hosts:
- cert_expires: Sep 13 02:52:55 2026 GMT
  host: www.azarahealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azara Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azara Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Azara Healthcare
provider_slug: azara-healthcare
slug: azara-healthcare-domain-security
source_filename: azara-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.azarahealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:52:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azarahealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azara-healthcare/refs/heads/main/security/azara-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Population Health
- Analytics
- Quality Reporting
- Community Health Centers
- Value-Based Care
- SDOH
---
