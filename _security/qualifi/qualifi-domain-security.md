---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qualifi.hr
  spf: true
hosts:
- cert_expires: Sep 25 11:35:48 2026 GMT
  host: www.qualifi.hr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualifi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qualifi
provider_slug: qualifi
slug: qualifi-domain-security
source_filename: qualifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualifi.hr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qualifi.hr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualifi/refs/heads/main/security/qualifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Hiring
- Human Resources
- HR Tech
- Interviewing
- Talent Acquisition
- ATS
---
