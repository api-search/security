---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: caremo.net
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: caremo.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caremo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caremo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Caremo
provider_slug: caremo
slug: caremo-domain-security
source_filename: caremo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caremo.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: caremo.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caremo/refs/heads/main/security/caremo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- HomeHealth
- Caregiving
- SeniorCare
- Therapy
- California
---
