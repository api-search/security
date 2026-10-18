---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: csvgateway.app
  spf: true
hosts:
- cert_expires: Dec 28 00:28:29 2026 GMT
  host: csvgateway.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Csvgateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CSV Gateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CSV Gateway
provider_slug: csvgateway
slug: csvgateway-domain-security
source_filename: csvgateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csvgateway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 00:28:29 2026 GMT\n  hsts: false\ndomains:\n- domain: csvgateway.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csvgateway/refs/heads/main/security/csvgateway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Integration
- No-Code
- API Generation
- CSV
- REST
- Software-as-a-Service
---
