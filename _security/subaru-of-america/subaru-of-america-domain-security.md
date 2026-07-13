---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: subaru.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.subaru.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Subaru Of America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subaru of America, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Subaru of America
provider_slug: subaru-of-america
slug: subaru-of-america-domain-security
source_filename: subaru-of-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subaru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: subaru.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subaru-of-america/refs/heads/main/security/subaru-of-america-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automobiles
- Automotive
- Cars
- Vehicles
- Connected Vehicle
- Telematics
- OEM
---
