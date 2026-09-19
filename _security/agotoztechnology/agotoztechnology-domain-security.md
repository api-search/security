---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agotoz.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.agotoz.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: openapi.agotoz.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agotoztechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgotoZ Technology, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgotoZ Technology
provider_slug: agotoztechnology
slug: agotoztechnology-domain-security
source_filename: agotoztechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agotoz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: openapi.agotoz.com\n  https: false\ndomains:\n- domain: agotoz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agotoztechnology/refs/heads/main/security/agotoztechnology-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- SD-WAN
- Network as a Service
- Network Acceleration
- Enterprise Networking
- CDN
- SASE
- DDoS Protection
- Cloud Connectivity
- Data-Center
- Telecommunications
---
