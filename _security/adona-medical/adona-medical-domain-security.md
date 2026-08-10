---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adonamed.com
  spf: true
hosts:
- cert_expires: Oct 14 23:14:10 2026 GMT
  host: adonamed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adona Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adona Medical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adona Medical
provider_slug: adona-medical
slug: adona-medical-domain-security
source_filename: adona-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adonamed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:14:10 2026 GMT\n  hsts: false\ndomains:\n- domain: adonamed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adona-medical/refs/heads/main/security/adona-medical-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Medical Technology
- Healthcare
- Cardiovascular
- Heart Failure
- Remote Patient Monitoring
- Clinical Stage
---
