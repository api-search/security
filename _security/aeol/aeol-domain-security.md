---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aeolkorea.co.kr
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.aeolkorea.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AEOL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AEOL
provider_slug: aeol
slug: aeol-domain-security
source_filename: aeol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeolkorea.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aeolkorea.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeol/refs/heads/main/security/aeol-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Advanced Materials
- Metal-Organic Frameworks
- Air Purification
- Ventilation
- Dehumidification
- Carbon Capture
- HVAC
- Manufacturing
- South Korea
---
