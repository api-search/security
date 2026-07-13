---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dentsply-sirona.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dscore.com
  spf: true
hosts:
- host: www.dentsply-sirona.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
- cert_expires: Aug  1 14:47:53 2026 GMT
  host: open.dscore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 08:27:40 2026 GMT
  host: api.dscore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dentsply Sirona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dentsply Sirona, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dentsply Sirona
provider_slug: dentsply-sirona
slug: dentsply-sirona-domain-security
source_filename: dentsply-sirona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dentsply-sirona.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\n- host: open.dscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 14:47:53 2026 GMT\n  hsts: false\n- host: api.dscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 08:27:40 2026 GMT\n  hsts: null\ndomains:\n- domain: dentsply-sirona.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: dscore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/security/dentsply-sirona-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CAD/CAM
- CEREC
- Dental
- DS Core
- Imaging
- Intraoral Imaging
- Lab Management
- Practice Management
- Fortune 1000
---
