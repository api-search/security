---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vishay.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nexar.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.vishay.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: nexar.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 18:01:53 2026 GMT
  host: developer.digikey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vishay Intertechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vishay Intertechnology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vishay Intertechnology
provider_slug: vishay-intertechnology
slug: vishay-intertechnology-domain-security
source_filename: vishay-intertechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vishay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: nexar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: developer.digikey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vishay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nexar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vishay-intertechnology/refs/heads/main/security/vishay-intertechnology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Capacitors
- Diodes
- Electronics
- Industrial
- MOSFETs
- Manufacturing
- Medical
- Optoelectronics
- Passive Components
- Resistors
- Semiconductors
- Fortune 1000
---
