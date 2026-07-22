---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: icontrolapp.se
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: icontrolapp.se
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Icontrol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iControl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: iControl
provider_slug: icontrol
slug: icontrol-domain-security
source_filename: icontrol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icontrolapp.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: icontrolapp.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icontrol/refs/heads/main/security/icontrol-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Construction
- Construction Technology
- Documentation
- Field Service
- Inspection
- Mobile
- Project Management
- Sweden
---
