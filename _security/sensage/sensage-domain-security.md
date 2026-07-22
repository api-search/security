---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sensage.com
  spf: false
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: sensage.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sensage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SenSage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SenSage
provider_slug: sensage
slug: sensage-domain-security
source_filename: sensage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensage.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sensage.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensage/refs/heads/main/security/sensage-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Security
- SIEM
- Log Management
- Security Analytics
- Event Data
- Compliance
- Defunct
---
