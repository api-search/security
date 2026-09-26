---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arincare.com
  spf: true
hosts:
- cert_expires: Nov  2 19:32:19 2026 GMT
  host: arincare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arincare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arincare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Arincare
provider_slug: arincare
slug: arincare-domain-security
source_filename: arincare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arincare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:32:19 2026 GMT\n  hsts: false\ndomains:\n- domain: arincare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arincare/refs/heads/main/security/arincare-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pharmacy
- DigitalHealth
- Thailand
- SaaS
---
